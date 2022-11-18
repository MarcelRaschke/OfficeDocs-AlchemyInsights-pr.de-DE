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
- "2556"
ms.openlocfilehash: 4a61777324c60ca6f7df82aed81c22236071bb46
ms.sourcegitcommit: 161627c9e0f44923e80332c9a8d12e40d838433c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/30/2022
ms.locfileid: "66565609"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Leerer Anmeldebildschirm in Microsoft 365-Apps

Um dieses Problem zu beheben, versuchen Sie Folgendes:
- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.microsoft.com/office/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Internet Explorer-Optionen zurücksetzen: Wechseln Sie zu **Extras** > **Internetoptionen** > **Advanced** > **Reset Internet Explorer Settings** (beachten Sie, dass Benutzerdefinierte Einstellungen verloren gehen), und versuchen Sie dann erneut, sich bei Office anzumelden.
- Deaktivieren Sie die Windows Defender Application Guard (WDAG) oder ein ähnliches Firewall- oder Antivirenprogramm:
    1. Wechseln Sie in Systemsteuerung zu **"Programme**", und wählen **Sie dann "Windows-Features aktivieren oder deaktivieren" aus**.
    2. Wenn Windows Defender Application Guard aktiviert ist, versuchen Sie, es zu deaktivieren.<br/>
    **Hinweis:** Möglicherweise müssen Sie den Computer neu starten.
- Stellen Sie sicher, dass das Microsoft.AAD.BrokerPlugin [AAD WAM-Plug-In](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nicht von einer Anwendung oder einem Firewall-/Antivirenprogramm blockiert wird.
- [Löschen Sie Die Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmeldeinformations-Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden in 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)

Weitere Informationen finden Sie [unter Verbindungsprobleme bei der Anmeldung nach dem Update auf Office 2016 Build 16.0.7967 auf Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).