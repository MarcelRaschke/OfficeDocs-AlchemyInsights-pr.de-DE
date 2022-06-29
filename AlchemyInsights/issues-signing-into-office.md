---
title: Probleme beim Anmelden bei Microsoft 365-Apps
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 6769038466c8ac33b2c6efc9236d7c1b94227722
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66258130"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Probleme beim Anmelden bei Microsoft 365 Apps

Hinweis: Wenn Sie eine ältere Version von Windows verwenden (z. B. Windows 7 SP1, Windows Server 2008 R2), verwenden Sie die [einfache Lösung](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) , um TLS 1.2 standardmäßig zu aktivieren. Weitere Informationen finden Sie unter [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Wenn Sie Probleme bei der Anmeldung bei den Microsoft 365-Apps beheben möchten, probieren Sie die folgenden Optionen auf dem betroffenen Computer:  

- Informationen zu Windows finden Sie unter [Empfehlungen zum Beheben häufiger Anmeldeprobleme](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues).
- Informationen für Mac finden [Sie unter "Anmelden bei einer Office 2016 für Mac-App nicht](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tipp** Auf Windows-Computern können wir mehrere häufige Probleme bei der Anmeldung bei Office für Sie diagnostizieren und automatisch beheben. Laden Sie den **[Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SaRA-OfficeSignInScenario)** herunter.

**Hinweis:** Das Deaktivieren der modernen Authentifizierung (ADAL) oder web account management (WAM) zum Beheben von Anmelde- oder Aktivierungsproblemen  **wird nicht empfohlen**. Wenn die Fehler beim Herstellen einer Verbindung mit Microsoft 365 mit Office 2013 auftreten, stellen Sie sicher, dass Sie die [moderne Authentifizierung](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  für den Office-Client aktivieren.

Spezifische Problembehandlungsaktionen finden Sie unter:

[Verbindungsprobleme bei der Anmeldung nach dem Update auf Office 2016, Build 16.0.7967, unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Sie können sich nicht bei Ihrem Organisationskonto wie Office 365, Azure oder Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Problembehandlung bei Nicht-Browser-Apps, die sich nicht bei Office 365, Azure oder Intune anmelden können](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Wiederholte Aufforderung zur Eingabe von Anmeldeinformationen in Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)