---
title: Probleme bei der Anmeldung bei Microsoft 365 Apps
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
  - 9000571
  - 2559
---

# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Beheben der Meldung "Das vertrauenswürdige Plattformmodul Ihres Computers funktioniert nicht ordnungsgemäß" Microsoft 365 Apps

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Löschen Sie Office Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) mit Windows Anmeldeinformations-Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Versuchen Sie den [Benutzerwiederherstellungsprozess,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) um TPM-Fehler (Trusted Platform Module) zu beheben.
- Legen Sie enableADAL = 0 fest, indem Sie die folgenden Schritte ausführen:  
    1. Klicken Sie mit der rechten Maustaste auf die Schaltfläche Windows Start, wählen Sie **"Ausführen",** geben Sie **"regedit"** ein, und klicken Sie dann auf **"OK".**
    2. Wählen Sie **"Ja"** aus, um dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu erlauben.
    3. Fügen Sie im Registrierungs-Editor einen DWORD-Wert von **EnableADAL** mit einer Einstellung von **0** unter HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity hinzu.

Weitere Informationen finden Sie unter Verbindungsprobleme bei der [Anmeldung nach dem Update auf Office 2016 Build 16.0.7967 auf Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).