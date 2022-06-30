---
title: 'Beheben der Microsoft 365-Apps: Ihr Konto befindet sich in einer Meldung in einem ungültigen Zustand'
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
- "2558"
ms.openlocfilehash: 3b888e54b620379ae2ec7674d3c2a2f87dffd3b1
ms.sourcegitcommit: 8324c868c664bfdee6d5bb99ad8d41e9dd46d10f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66539234"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Beheben des Fehlers "Ihr Konto befindet sich in einem schlechten Zustand" in Microsoft 365-Apps

Um diesen Fehler zu beheben, probieren Sie die folgenden Optionen auf dem betroffenen Computer aus:

- Öffnen Sie eine Office-App **, und wählen** Sie  >  "**Dateikonto** > **abmelden" für alle Konten aus**. Melden Sie sich mit einem Benutzerkonto mit einer gültigen Lizenz erneut an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.microsoft.com/office/about-accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Löschen Sie Die Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmeldeinformations-Manager.<br>
  **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\
- Wenn der Fehler beim Herstellen einer Verbindung mit Office 365 mit Office 2013 auftritt, [aktivieren Sie die moderne Authentifizierung](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) für den Office-Client.

Weitere Informationen finden Sie unter [Problembehandlung bei Nicht-Browser-Apps, die sich nicht bei Microsoft 365, Azure oder Intune anmelden können](https://support.microsoft.com/office/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-microsoft-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

