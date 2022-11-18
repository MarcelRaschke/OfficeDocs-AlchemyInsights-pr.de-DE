---
title: Gerät im Status "Ausstehend"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 37fb1089632615cae04515482f5f5bdcaf2f575d
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66519141"
---
# <a name="device-in-pending-state"></a>Gerät im Status "Ausstehend"

**Voraussetzungen:**

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die [Einführung in die Geräteverwaltung in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) überprüft haben, die Sie beim Abrufen von Geräten unter die Kontrolle von Azure AD führt.
2. Wenn Sie Geräte direkt bei Azure AD registrieren und bei Intune registrieren, müssen Sie sicherstellen, dass Sie [Intune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) haben und zuerst über die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) verfügen.
3. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD und lokalen AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten. Wenn Sie außerdem automatische Registrierungen in Ihrem lokalen Active Directory einrichten, müssen Sie außerdem Administrator von Active Directory und (sofern zutreffend) AD FS sein.

Für den Azure AD-Hybridregistrierungsprozess müssen sich Geräte im Unternehmensnetzwerk befinden. Es funktioniert auch über VPN, aber es gibt einige Einschränkungen. Wir haben gehört, dass Kunden Unterstützung bei der Problembehandlung beim Hybrid-Azure AD-Registrierungsprozess unter Remotearbeitsverhältnissen benötigen.

**Cloudauthentifizierungsumgebung (mithilfe der Azure AD-Kennworthashsynchronisierung oder Pass-Through-Authentifizierung)**

Dieser Registrierungsfluss wird auch als "Sync Join" bezeichnet.

Hier ist eine Aufschlüsselung, was während des Registrierungsprozesses geschieht:

1. Windows 10 ermittelt den Dienstverbindungspunkt(SCP)-Eintrag, wenn sich der Benutzer beim Gerät anmeldet.

    1. Das Gerät versucht zuerst, Mandanteninformationen von clientseitigem SCP in der Registrierung abzurufen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Weitere Informationen finden Sie im [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Wenn ein Fehler auftritt, kommuniziert das Gerät mit lokales Active Directory, um Mandanteninformationen von SCP abzurufen. Informationen zum Überprüfen von SCP finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    **Hinweis**: Es wird empfohlen, SCP im Active Directory zu aktivieren und nur clientseitiges SCP für die anfängliche Überprüfung zu verwenden.

2. Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich gegenüber Azure AD zu authentifizieren.

    Sie können mithilfe des [Skripts "Geräteregistrierungskonnektivität](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0) testen" überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann.

3. Windows 10 generiert ein selbstsigniertes Zertifikat und speichert es unter dem Computerobjekt in lokales Active Directory. Dies erfordert eine Sichtweite zum Domänencontroller.

4. Geräteobjekt mit Zertifikat wird über Azure AD Connect mit Azure AD synchronisiert. Der Synchronisierungszyklus erfolgt standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration von Azure AD Connect ab. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. In dieser Phase sollten Sie das Betreffgerät im Status "**Ausstehend**" unter dem Geräteblatt des Azure-Portals sehen können.

6. Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen.

    **Hinweis**: Wenn Sie ein VPN verwenden und die Domänenkonnektivität durch Abmeldung/Anmeldung beendet wird, können Sie die Registrierung manuell auslösen. Gehen Sie dazu wie folgt vor:
    
    Stellen Sie lokal eine `dsregcmd /join` Administratoraufforderung oder remote über PSExec auf Ihren PC aus.\
    Beispiel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Allgemeine Probleme bei der Azure Active Directory-Geräteregistrierung finden Sie unter [Häufig gestellte Fragen zu Geräten](https://docs.microsoft.com/azure/active-directory/devices/faq).
