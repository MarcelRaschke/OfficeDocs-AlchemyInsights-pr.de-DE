---
title: Probleme bei der Anmeldung bei Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695322"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Beheben der Microsoft 365-Apps "Sorry, ein anderes Konto aus Ihrer Organisation ist bereits angemeldet" Nachricht

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Entfernen Sie alle Arbeits Konten außer dem betroffenen Konto mithilfe von Windows-Einstellungen > **Access work oder School**.
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öffnen Sie eine Office-App, und wählen Sie **Datei**  >  **Konto**  >  **Abmelden aus**. Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Weitere Informationen finden Sie unter ["Sorry, ein anderes Konto aus Ihrer Organisation ist bereits auf diesem Computer angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).