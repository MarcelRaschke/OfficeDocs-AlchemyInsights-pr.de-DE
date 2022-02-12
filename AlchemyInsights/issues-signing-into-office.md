---
title: Probleme bei der Anmeldung bei Microsoft 365-Apps
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: d4ea0d863514c65d13da7b81358d4f7fc7620d7c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62590654"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Probleme bei der Anmeldung bei Microsoft 365 Apps

Hinweis: Wenn Sie eine ältere Version von Windows verwenden (z. B. Windows 7 SP1, Windows Server 2008 R2), verwenden Sie die [einfache Korrektur](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi), um TLS 1.2 standardmäßig zu aktivieren. Weitere Informationen finden Sie unter [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Wenn Sie Probleme bei der Anmeldung bei den Microsoft 365-Apps beheben möchten, probieren Sie die folgenden Optionen auf dem betroffenen Computer:  

- Informationen zu Windows finden Sie unter [Empfehlungen zur Behebung allgemeiner Anmeldeprobleme](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues).
- Informationen zu Mac finden Sie unter ["Kann sich nicht bei einer Office 2016 für Mac-App anmelden](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)"

**Tipp** Auf Windows-Computern können wir mehrere häufige Probleme bei der Anmeldung bei Office für Sie diagnostizieren und automatisch beheben. Laden Sie den **[Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SaRA-OfficeSignInScenario)** herunter.

**Hinweis:** Das Deaktivieren der modernen Authentifizierung (Modern Authentication, ADAL) oder der Web Account Management (WAM) zum Beheben von Anmelde- oder Aktivierungsproblemen  **wird nicht empfohlen**. Wenn die Fehler beim Herstellen einer Verbindung mit Microsoft 365 mit Office 2013 auftreten, stellen Sie sicher, dass Sie die [moderne Authentifizierung](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) für Office Client aktivieren.

Spezifische Problembehandlungsaktionen finden Sie unter:

[Verbindungsprobleme bei der Anmeldung nach dem Update auf Office 2016, Build 16.0.7967, unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Sie können sich nicht bei Ihrem Organisationskonto anmelden, z. B. Office 365, Azure oder Intune.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Problembehandlung bei Nicht-Browser-Apps, die sich nicht bei Office 365, Azure oder Intune anmelden können](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Wiederholte Aufforderung zur Eingabe von Anmeldeinformationen in Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)