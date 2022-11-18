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
- "2559"
ms.openlocfilehash: fc2b4e3ae1c95e63d9bdae9dd66b1b5f7da628d2
ms.sourcegitcommit: 161627c9e0f44923e80332c9a8d12e40d838433c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/30/2022
ms.locfileid: "66566761"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Beheben der Meldung "Das Modul der vertrauenswürdigen Plattform Ihres Computers funktioniert nicht ordnungsgemäß" in Microsoft 365-Apps

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.microsoft.com/office/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Löschen Sie Die Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) mit dem Windows-Anmeldeinformations-Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Versuchen Sie es mit dem [Benutzerwiederherstellungsprozess](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , um TPM-Fehler (Trusted Platform Module) zu beheben.
- Legen Sie "EnableADAL = 0" mit den folgenden Schritten fest:  
    1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche "Start", wählen Sie " **Ausführen**", geben **Sie "regedit"** ein, und wählen Sie dann **"OK**" aus.
    2. Wählen Sie **"Ja** " aus, damit der Registrierungs-Editor Änderungen an Ihrem Gerät vornehmen kann.
    3. Fügen Sie im Registrierungs-Editor einen DWORD-Wert von **EnableADAL** mit der Einstellung **0** unter HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity hinzu.

Weitere Informationen finden Sie [unter Verbindungsprobleme bei der Anmeldung nach dem Update auf Office 2016 Build 16.0.7967 auf Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).