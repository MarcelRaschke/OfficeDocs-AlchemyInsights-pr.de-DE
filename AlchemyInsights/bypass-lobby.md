---
title: Steuern der Lobbyeinstellungen und des Umfangs der Teilnahme an Teams
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 5e36794183b5453c326a5ecfa29630dc2482aad5
ms.sourcegitcommit: 8515ab69b43b47aaf3c5d1901fc398e8e26e618c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/17/2021
ms.locfileid: "61558814"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Steuern der Lobbyeinstellungen und des Umfangs der Teilnahme an Teams

Zwei Steuerungsebenen bestimmen die Lobbyumgebung für Teams Besprechungsteilnehmer: Besprechungsrichtlinien pro Organisator und Besprechungsoptionen.  

Administratoren verwenden die folgenden organisatorbasierten Richtlinien, um zu steuern, welche Besprechungsteilnehmer im Wartebereich warten, bevor sie zur Besprechung zugelassen werden:

- [Personen automatisch zulassen](https://docs.microsoft.com/microsoftteams/meeting-policies-participants-and-guests#automatically-admit-people)
- [Anonymen Personen das Starten einer Besprechung gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-participants-and-guests#let-anonymous-people-start-a-meeting)
- [Einwählbenutzern das Umgehen des Wartebereichs gestatten](https://docs.microsoft.com/microsoftteams/meeting-policies-participants-and-guests#allow-dial-in-users-to-bypass-the-lobby)  

Administratoren können diese Einstellungen im Teams Admin Center oder über PowerShell aktivieren. Weitere Informationen finden Sie unter [Aktivieren von Besprechungsrichtlinieneinstellungen.](https://docs.microsoft.com/microsoftteams/meeting-policies-participants-and-guests#enable-meeting-policy-settings)  

Nachdem Sie eine Richtlinie eingerichtet und auf Benutzer angewendet haben, müssen Sie 4 bis 24 Stunden warten, bis die Richtlinien wirksam werden.  

Besprechungsorganisatoren können **steuern, Wer den Wartebereich umgehen können,** und **Anrufer den Wartebereich immer** über **Besprechungsoptionen** pro Besprechung umgehen lassen. Mit diesen Besprechungsoptionen können Besprechungsorganisatoren die Richtlinie **"Personen automatisch zulassen"** außer Kraft setzen, und die **Einwahlbenutzer können die Lobbyrichtlinie** für eine bestimmte Besprechung umgehen. Weitere Informationen finden Sie unter [Ändern der Teilnehmereinstellungen für eine Teams Besprechung.](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)