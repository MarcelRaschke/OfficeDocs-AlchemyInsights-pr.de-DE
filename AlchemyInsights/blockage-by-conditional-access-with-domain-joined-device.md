---
title: Ich werde durch den bedingten Zugriff mit einem in der Domäne eingebunden Gerät blockiert
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: abef2a3d10c0f5c68e91a671934473e48f33c4b3
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63195404"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Ich werde durch den bedingten Zugriff mit einem in der Domäne eingebunden Gerät blockiert

**Sehr empfehlenswerte Tools**

[Problembehandlungstool für Geräteregistrierungen](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Ein Tool zur Behebung der häufigsten Probleme bei der Geräteregistrierung.

[Skript zum Testen der Verbindung der Geräteregistrierung](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Ein Skript, mit dem sichergestellt wird, dass ein Gerät unter dem Systemkonto auf Endpunkte der Geräteregistrierung zugreifen kann.

[Azure AD-Gerätebereinigungsskript](https://github.com/mzmaili/AzureADDeviceCleanup) – Ein Skript, um veraltete Geräte in Ihrer Umgebung aufzufinden und zu verwalten.

Hier finden Sie einige häufige Ursachen, warum der bedingte Zugriff bei einem Gerät, das in einer Domäne eingebunden ist, (Azure AD Hybrid), fehlgeschlagen ist.

1. **Es gibt kein Azure AD-PRT auf dem Gerät** – Sie müssen sicherstellen, dass das Gerät über das primäre Azure AD-Aktualisierungstoken (PRT) verfügt. Weitere Informationen zum PRT finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Um zu überprüfen, ob Sie über das Azure AD-PRT verfügen, können Sie den `dsregcmd/status`-Befehl auf dem Gerät ausführen. Überprüfen Sie, ob „AzureAdPrt“ gleich „JA“ ist.

Wenn „AzureAdPrt“ gleich „NEIN“ ist, überprüfen Sie Folgendes:

- **Unabhängig davon, ob Sie über eine Verbundumgebung mit ADFS verfügen und diese von den Heimnetzwerken Ihrer Benutzer nicht erreichbar ist**: Stellen Sie in diesem Fall sicher, dass über das Extranet auf Ihre „usernamemixed“-Endpunkte zugegriffen werden kann. Wenn sich Ihre ADFS hinter einem VPN befinden, stellen Sie sicher, dass sich die Benutzer mit dem VPN verbinden und sich erneut auf dem Gerät anmelden. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Führen Sie Folgendes durch, wenn das TPM des Geräts fehlerhaft ist und es daher nicht authentifiziert werden kann**: Überprüfen Sie „tpm.msc“, um herauszufinden, ob der Status von TPM „Bereit“ ist. Falls dies nicht der Fall ist, führen Sie den Befehl `dsregcmd/leave` aus, und lassen Sie das Gerät wieder mit Azure AD verknüpfen. Führen Sie den Vorgang anschließend erneut aus. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Sie verwenden einen Identitätsanbieter eines Drittanbieters, der das WS-Trust-Protokoll nicht unterstützt**. Wie in unseren Dokumenten beschrieben, können mit Azure AD Hybrid verbundene Geräte in diesem Fall nicht funktionieren. Wenden Sie sich an Ihren Identitätsanbieter, um Unterstützung zu erhalten.

2. **Benutzer verwenden den Chrome-Browser ohne die Windows 10-Konten** oder **Office-Erweiterung; Chrome verwendet den PRT nicht automatisch bei mit AAD oder AAD Hybrid verbundenen Geräten**: Dies führt zu einem Fehler bei allen gerätebasierten Richtlinien für den bedingten Zugriff, und die Fehlermeldung „Nicht registriertes Gerät“ wird angezeigt. Damit Sie den Chrome-Browser ordnungsgemäß verwenden können, müssen Sie die „Windows 10-Konten“ oder die „Office-Erweiterung des Chrome-Browsers der Benutzer“ über den SCCM oder Intune installieren. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Wenn es nicht möglich ist, die Erweiterung remote zu übertragen, benachrichtigen Sie die Benutzer, eine der oben genannten Erweiterungen manuell zu installieren, um hinter dem gerätebasierten bedingten Zugriff auf Anwendungen zu zugreifen. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Das Gerät war ordnungsgemäß in Azure AD Hybrid eingebunden, wurde aber versehentlich gelöscht oder deaktiviert, entweder aufgrund von Synchronisierungsänderungen in Azure AD Connect oder über das Azure-Portal**: In diesem Fall wird das Geräteobjekt nicht mehr als vollständig eingebundenes Gerät erkannt, obwohl die Status „AzureAdJoined“ und „PRT“ auf dem Gerät als gültig angezeigt werden.

Um dieses Problem zu beheben, führen Sie den `dsregcmd/leave`-Befehl auf den betroffenen Geräten aus, und lassen Sie sie wieder mit Azure AD verknüpfen. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

**Hinweis**: Wenn Ihre Geräte unter Windows 10, Version 1809, mit VPN/Cloud-Proxy laufen und Probleme mit dem Status „AzureAdPrt“ oder bei einer beliebigen App Probleme mit SSO auftreten (Outlook konnte keine Verbindung mit Postfach herstellen, obwohl PRT verwendet wurde), stellen Sie sicher, dass Sie über dieses Patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) oder das kumulative April-Update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) verfügen, um PRT-Fehler auf diesen Geräten zu verhindern.

















