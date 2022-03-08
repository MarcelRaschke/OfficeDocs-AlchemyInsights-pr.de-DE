---
title: Probleme bei der Anmeldung bei Microsoft 365-Apps
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 8340958bae92818f935c65e427a147dedb76e9bf
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63214557"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Leerer Anmeldebildschirm in Microsoft 365-Apps

Um dieses Problem zu beheben, versuchen Sie Folgendes:
- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Internet Explorer-Optionen zurücksetzen: Wechseln Sie zu **ToolsInternet** >  **OptionsAdvancedReset** >  >  **Internet Explorer-Einstellungen** (beachten Sie, dass benutzerdefinierte Einstellungen verloren gehen), und versuchen Sie dann erneut, sich bei Office anzumelden.
- Deaktivieren Sie Windows Defender Application Guard (WDAG) oder ähnliche Firewall- oder Antivirenprogramme:
    1. Wechseln Sie in der Systemsteuerung zu **"Programme**", und wählen Sie " **Windows-Features aktivieren oder deaktivieren" aus**.
    2. Wenn Windows Defender Application Guard aktiviert ist, versuchen Sie, es zu deaktivieren.<br/>
    **Hinweis:** Möglicherweise müssen Sie den Computer neu starten.
- Stellen Sie sicher, dass das Microsoft.AAD.BrokerPlugin [AAD WAM-Plug-In](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nicht durch eine Anwendung oder ein Firewall-/Antivirenprogramm blockiert wird.
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmeldeinformations-Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden zu 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)

Weitere Informationen finden Sie unter [Verbindungsprobleme bei der Anmeldung nach dem Update auf Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).