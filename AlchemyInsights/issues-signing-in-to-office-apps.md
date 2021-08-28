---
title: Probleme beim Anmelden bei Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028039"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Beheben der Meldung "Leider ist ein anderes Konto aus Ihrer Organisation bereits angemeldet" Microsoft 365 Apps

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Entfernen Sie alle Geschäftskonten mit Ausnahme des betroffenen Kontos, indem Sie Windows Einstellungen > **Auf Arbeits- oder Schulkonto zugreifen.**
- [Löschen Sie Office Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit Windows Anmeldeinformations-Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öffnen Sie eine Office-App, wählen Sie **"Dateikonto**  >    >  **abmelden" aus.** Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Weitere Informationen finden Sie unter ["Leider ist ein anderes Konto aus Ihrer Organisation bereits auf diesem Computer angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).