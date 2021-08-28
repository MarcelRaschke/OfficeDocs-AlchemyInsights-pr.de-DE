---
title: Umgehen des Wartebereichs
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
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059595"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Steuern der Lobbyeinstellungen und des Grads der Teilnahme an Teams

Wenn Sie zulassen möchten, dass jeder, einschließlich Einwahl, externer und anonymer Benutzer, **den Wartebereich umgehen** kann, verwenden Sie PowerShell, um diese Aufgabe zu erledigen. Hier ist ein Beispiel zum Ändern der globalen Besprechungsrichtlinie für Ihre Organisation.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Dieses Cmdlet erfordert derzeit die Verwendung Skype for Business PowerShell-Moduls. Informationen zum Einrichten der Verwendung dieses Cmdlets finden Sie unter [Verwalten von Richtlinien über PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Nachdem Sie eine Richtlinie eingerichtet haben, müssen Sie sie auf Benutzer anwenden. oder wenn Sie die globale Richtlinie geändert haben, gilt sie automatisch für Benutzer. Für jede Richtlinienänderung müssen Sie mindestens **4 Stunden bis zu 24 Stunden** warten, bis die Richtlinien wirksam werden. 

Überprüfen Sie unbedingt die nachstehende Dokumentation, bevor Sie diese Änderungen vornehmen, um genau zu verstehen, was dies zulässt.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Grundlegendes zu richtliniensteuerungen für Teams Besprechungslobby

Diese Einstellungen steuern, welche Besprechungsteilnehmer im Wartebereich warten, bevor sie zur Besprechung zugelassen werden, und welche Teilnahmestufe sie an einer Besprechung haben. Sie können PowerShell verwenden, um Besprechungsrichtlinieneinstellungen zu aktualisieren, die noch nicht im Teams Admin Center implementiert wurden (mit der Bezeichnung "in Kürze verfügbar"). Ein Beispiel für ein PowerShell-Cmdlet, mit dem alle Benutzer den Wartebereich umgehen können, finden Sie unten.

- ["Personen automatisch zulassen"](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) ist eine organisatorspezifische Richtlinie, die steuert, ob Personen direkt an einer Besprechung teilnehmen oder im Wartebereich warten, bis sie von einem authentifizierten Benutzer zugelassen werden.

- [Anonymen Personen das Starten einer Besprechung zu gestatten,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ist eine organisatorspezifische Richtlinie, die steuert, ob anonyme Personen, einschließlich B2B- und Verbundbenutzer, an der Besprechung des Benutzers teilnehmen können, ohne dass ein authentifizierter Benutzer aus der Organisation anwesend ist.

- [Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ( coming **soon**) is a pro-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the Automatically **admit people** setting.

- Zulassen, dass Organisatoren Lobbyeinstellungen außer Kraft setzen (**in Kürze verfügbar)** ist eine organisatorspezifische Richtlinie, die steuert, ob der [Besprechungsorganisator](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) die Lobbyeinstellungen außer Kraft setzen kann, die ein Administrator unter **"Personen automatisch zulassen"** und **Einwahlbenutzern die Umgehung des Wartebereichs gestatten** kann, wenn sie eine neue Besprechung planen.

**Hinweis:** Eine vollständige Übersicht über Microsoft Teams Besprechungsrichtlinien finden Sie unter Verwalten von [Besprechungsrichtlinien in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)
