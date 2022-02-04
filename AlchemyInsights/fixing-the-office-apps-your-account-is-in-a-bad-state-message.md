---
title: 'Beheben der Microsoft 365 Apps, für die Ihr Konto in einer Meldung mit ungültigen Zuständen angezeigt wird'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
  - 2558
  - 9000571
---

# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Beheben des Fehlers "Ihr Konto befindet sich in einem ungültigen Zustand" Microsoft 365 Apps

Um diesen Fehler zu beheben, versuchen Sie die folgenden Optionen auf dem betroffenen Computer:

- Öffnen Sie eine Office-App, wählen Sie **"Dateikonto**  >    >  **abmelden" aller Konten aus.** Melden Sie sich mit einem Benutzerkonto mit einer gültigen Lizenz erneut an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Löschen Sie Office Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit Windows Anmeldeinformations-Manager.<br>
  **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\
- Wenn der Fehler beim Herstellen einer Verbindung mit Office 365 mit Office 2013 auftritt, aktivieren Sie die [moderne Authentifizierung](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) für den Office Client.

Weitere Informationen finden Sie unter [Problembehandlung bei Nicht-Browser-Apps, die sich nicht bei Microsoft 365, Azure oder Intune anmelden können.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

