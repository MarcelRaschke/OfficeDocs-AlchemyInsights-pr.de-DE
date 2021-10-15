---
title: Bei einigen Benutzern kann es zu Verzögerungen bei Chatnachrichten kommen.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000738"
- "8431"
ms.openlocfilehash: 08675d419ed25c31ad35c2432be83ca943a2fd3f
ms.sourcegitcommit: ae8fed7a78ea7c8680d8348b05400dd31f3bde91
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370757"
---
# <a name="some-users-may-experience-delays-with-chat-messages"></a>Bei einigen Benutzern kann es zu Verzögerungen bei Chatnachrichten kommen.

Bei einigen Microsoft Teams Benutzern können fehlende Nachrichten oder Verzögerungen beim Senden und Empfangen von Chatnachrichten auftreten.

Überprüfen Sie im Microsoft Admin Center > [**Dienststatus,**](https://admin.microsoft.com/servicehealth) ob kein aktives Problem für Microsoft Teams vorliegt.

Überprüfen Sie, ob das Problem für [Teams im Web](https://teams.microsoft.com/)weiterhin besteht. Wenn das Problem nur für die Teams Desktopversion auftritt:

1. Melden Sie sich von Teams auf dem Desktop ab.

1. Löschen Sie den Cache. Auf einem Windows Desktop:

    1. Halten Sie auf der Tastatur die Windows Taste gedrückt, und drücken Sie **R.**

    1. **%appdata%\Microsoft\Teams** ausschneiden und einfügen > **OK** auswählen.
    1. Löschen Sie den Inhalt dieser Ordner: BLOB-Speichercachedatenbanken GPUCache IndexedDB Local Storage tmp

3. Starten Sie Microsoft Teams > Anmelden neu.

Weitere Informationen zu Teams Clientupdates und zur Problembehandlung Microsoft Teams Installation finden Sie unter:

- [Teams Aktualisierungsprozess](https://docs.microsoft.com/microsoftteams/teams-client-update)
- [Problembehandlung bei Microsoft Teams Installations- und Updateproblemen bei Windows](https://docs.microsoft.com/microsoftteams/troubleshoot-installation)


