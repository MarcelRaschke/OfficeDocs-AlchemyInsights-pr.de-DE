---
title: Problembehandlung beim PRT-Problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972715"
---
# <a name="troubleshoot-prt-issue"></a>Problembehandlung beim PRT-Problem

Damit alle Geräte authentifiziert werden können, muss es vollständig registriert und in gutem Zustand sein und in der Lage sein, ein primäres Aktualisierungstoken (PRT) zu erhalten.

Der Azure AD-Hybridregistrierungsprozess erfordert, dass sich Geräte in einem Unternehmensnetzwerk befinden. Es funktioniert auch über VPN, aber es gibt einige Einschränkungen. Wir haben gehört, dass Kunden Unterstützung bei der Problembehandlung beim Azure AD-Hybridregistrierungsprozess unter Remotearbeitsumgebungen benötigen. Nachfolgend finden Sie eine Aufschlüsselung der Vorgänge während des Registrierungsprozesses "im Hintergrund".

**Cloudauthentifizierungsumgebung (mit azure AD-Kennworthashsynchronisierung oder Pass-Through-Authentifizierung)**

Dieser Registrierungsfluss wird auch als "Sync Join" bezeichnet.

1. Windows 10 ermittelt einen SCP-Eintrag, wenn sich der Benutzer beim Gerät anmeldet.
    1. Das Gerät versucht zunächst, Mandanteninformationen von clientseitigem SCP in der Registrierung [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] abzurufen. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Wenn ein Fehler auftritt, kommuniziert das Gerät mit dem lokalen Active Directory (AD), um Mandanteninformationen vom Dienstverbindungspunkt (Service Connection Point, SCP) abzurufen. Informationen zur Überprüfung von SCP finden Sie in diesem [Dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Es wird empfohlen, SCP im AD zu aktivieren und nur clientseitige SCP für die anfängliche Überprüfung zu verwenden.

2. Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich bei Azure AD zu authentifizieren. Sie können überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann, indem Sie das Skript "Geräteregistrierungskonnektivität testen" verwenden.

3. Windows 10 generiert ein selbstsignantes Zertifikat und speichert es unter dem Computerobjekt im lokalen AD. Dies erfordert eine Sichtachse für den Domänencontroller.

4. Ein Geräteobjekt, das über ein Zertifikat verfügt, wird über Azure AD Verbinden mit Azure AD synchronisiert. Der Synchronisierungszyklus erfolgt standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration der Azure AD-Verbinden ab. Weitere Informationen finden Sie in diesem [Dokument.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. In dieser Phase sollten Sie das Betreffgerät im Status "Ausstehend" unter dem Blatt "Gerät" des Azure-Portals sehen können.

6. Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen. 

> [!NOTE]
> Wenn Sie sich auf einem VPN befinden und die Domänenkonnektivität durch einen Anmeldevorgang beendet wird, können Sie die Registrierung manuell auslösen:
 1. Geben Sie einen dsregcmd /join lokal auf Administratoraufforderung oder remote über PSExec an Ihren PC aus. Beispiel: PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Weitere Informationen zu Problemen beim Hybridbeitritt finden Sie unter [Problembehandlung bei Geräten.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
