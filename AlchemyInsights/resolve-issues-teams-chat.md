---
title: Beheben von Problemen mit Teams Chat
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
- "9000738"
- "16637"
ms.date: 02/07/2022
ms.openlocfilehash: 8218a7de5b3e5e5cbaabe585004abbc8862aac68
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63125165"
---
# <a name="resolve-issues-with-teams-chat"></a>Beheben von Problemen mit Teams Chat

Wenn Microsoft Teams Chat für einen oder mehrere Benutzer nicht verfügbar ist, überprüfen Sie zunächst Teams Richtlinieneinstellungen:

- Überprüfen Sie in der [Messagingrichtlinie](https://admin.teams.microsoft.com/policies/messaging) für den betroffenen Benutzer, ob "Chat" auf " **Ein**" festgelegt ist. Stellen Sie für Gastbenutzer sicher, dass der Chat in der [Gastzugriffsrichtlinie](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) **aktiviert** ist.

- Während einer Besprechung wird der Chat in der [Besprechungsrichtlinie aktiviert, die dem Benutzer zugewiesen](https://admin.teams.microsoft.com/policies/meetings) ist.

- Um einem Benutzer zugewiesene Richtlinien anzuzeigen, suchen Sie den Benutzer in **UserManage** >  **UsersView-Richtlinien**[](https://admin.teams.microsoft.com/users) > .

Besprechungsteilnehmer können während oder nach einer Besprechung ein fehlendes Chatsymbol oder einen fehlenden Chatverlauf feststellen, wenn das Besprechungslimit für Teilnehmer erreicht ist, ein Benutzer der Besprechung als "Anonym" beigetreten ist oder wenn ein Teilnehmer einen Link zur Teilnahme an einer Besprechung erhalten hat. Weitere Informationen finden Sie unter [Chat in einer Teams Besprechung](https://support.microsoft.com/office/chat-in-a-teams-meeting-64e2cb91-8a11-4781-94ea-fbb23f2b922f) und [Chatprobleme in Teams Besprechung](https://docs.microsoft.com/microsoftteams/troubleshoot/meetings/meeting-chat-issues).

Um Informationen in Ihrer Organisation zu verwalten, können Sie Aufbewahrungsrichtlinien erstellen und verwalten. Weitere Informationen finden Sie unter [Verwalten von Aufbewahrungsrichtlinien für Microsoft Teams](https://docs.microsoft.com/microsoftteams/retention-policies).
