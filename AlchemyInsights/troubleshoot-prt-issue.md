---
title: Problembehandlung bei PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: c598e4375f90d58496d05c6b6755adbc04ceb463
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65723288"
---
# <a name="troubleshoot-prt-issue"></a>Problembehandlung bei PRT

Damit jedes Gerät authentifiziert wird, muss es vollständig registriert und in gutem Zustand sein und in der Lage sein, ein primäres Aktualisierungstoken (Primary Refresh Token, PRT) zu erhalten.

Für den hybriden Azure AD-Registrierungsprozess müssen sich Geräte in einem Unternehmensnetzwerk befinden. Es funktioniert auch über VPN, aber es gibt einige Einschränkungen. Wir haben gehört, dass Kunden Unterstützung bei der Problembehandlung beim Hybrid-Azure AD-Registrierungsprozess unter Remotearbeitssituationen benötigen. Hier ist eine Aufschlüsselung dessen, was während des Registrierungsprozesses "unter der Haube" geschieht.

**Cloudauthentifizierungsumgebung (mithilfe der Azure AD-Kennworthashsynchronisierung oder Pass-Through-Authentifizierung)**

Dieser Registrierungsfluss wird auch als "Sync Join" bezeichnet.

1. Windows 10 erkennt einen SCP-Eintrag, wenn sich der Benutzer beim Gerät anmeldet.
   1. Das Gerät versucht zuerst, Mandanteninformationen von clientseitigem SCP in der Registrierung abzurufen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
   2. Wenn ein Fehler auftritt, kommuniziert das Gerät mit lokales Active Directory (AD), um Mandanteninformationen vom Dienstverbindungspunkt (Service Connection Point, SCP) abzurufen. Informationen zum Überprüfen von SCP finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

   **Hinweis**: Wir empfehlen, SCP im AD zu aktivieren und nur clientseitiges SCP für die anfängliche Überprüfung zu verwenden.

2. Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich gegenüber Azure AD zu authentifizieren. Sie können mithilfe des Skripts "Geräteregistrierungskonnektivität testen" überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann.

3. Windows 10 generiert ein selbstsigniertes Zertifikat und speichert es unter dem Computerobjekt in lokalem AD. Dies erfordert eine Sichtweite zum Domänencontroller.

4. Ein Geräteobjekt mit einem Zertifikat wird über Azure AD Verbinden mit Azure AD synchronisiert. Der Synchronisierungszyklus erfolgt standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration von Azure AD Verbinden ab. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. In dieser Phase sollten Sie das Betreffgerät im Status "Ausstehend" unter dem Geräteblatt des Azure-Portals sehen können.

6. Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen.

**Hinweis**: Wenn Sie ein VPN verwenden und ein Anmeldevorgang die Domänenkonnektivität beendet, können Sie die Registrierung manuell auslösen:

 1. Stellen Sie ein dsregcmd /join lokal an der Administratoraufforderung oder remote über PSExec auf Ihrem PC aus. Beispiel: PsExec -s \\win10client01 cmd, dsregcmd /join

 2. Weitere Informationen zu Problemen beim Hybridbeitritt finden Sie [unter Problembehandlung für Geräte](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
