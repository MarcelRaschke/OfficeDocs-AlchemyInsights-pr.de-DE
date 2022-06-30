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
- "2560"
ms.openlocfilehash: d0cc41a1419122f8b8d5f9c79973cb8529bec7d5
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66338781"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Beheben der Meldung "Leider ist ein anderes Konto aus Ihrer Organisation bereits angemeldet" in Microsoft 365-Apps

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Entfernen Sie alle Geschäftskonten, mit Ausnahme des betroffenen Kontos, mithilfe von Windows-Einstellungen > **Auf Geschäfts-, Schul- oder Unikonto zugreifen**.
- [Löschen Sie Die Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmeldeinformations-Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öffnen Sie eine Office-App, und wählen Sie **"** > **Dateikonto abmelden****"** >  aus. Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Weitere Informationen finden Sie [unter "Leider ist ein anderes Konto aus Ihrer Organisation bereits auf diesem Computer angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).