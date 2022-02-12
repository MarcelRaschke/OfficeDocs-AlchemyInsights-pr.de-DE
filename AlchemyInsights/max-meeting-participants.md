---
title: Maximale Anzahl von Besprechungsteilnehmern
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
- "9003355"
- "15557"
ms.openlocfilehash: da39e73fa5135b5ed61e411034db48d20cbf726f
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62698712"
---
# <a name="maximum-number-of-meeting-participants"></a>Maximale Anzahl von Besprechungsteilnehmern

Die maximale Anzahl von Teilnehmern pro Besprechung beträgt 1.000 für die meisten Lizenzen (A1-Lizenzen erlauben nur 300 Teilnehmer). Darüber hinaus können bis zu 10.000 Teilnehmer (bis zu 20.000 während 2021) an einer Besprechung teilnehmen, in der der Organisator über eine Lizenz für E3/E5/A3/A5 oder Government (GCC, GCC High, DoD) verfügt.

Die schreibgeschützte Oberfläche ermöglicht es den ersten 1.000 Teilnehmern, an der vollständigen Teams Besprechungserfahrung von Audio, Video und Chat teilzunehmen. Benutzer, die über die ersten 1.000 und bis zu 10.000 (20.000 im Jahr 2021) hinausgehen, haben eine schreibgeschützte Erfahrung. Die Schreibschutzumgebung ist standardmäßig deaktiviert und kann mithilfe dieses Teams PowerShell-Cmdlets aktiviert werden:

`Set-CsTeamsMeetingPolicy -Identity Global -StreamingAttendeeMode Enabled`

Weitere Informationen zur schreibgeschützten Benutzeroberfläche finden Sie unter [Teams schreibgeschützten Besprechungsoberfläche](https://docs.microsoft.com/microsoftteams/view-only-meeting-experience).

Die maximale Anzahl von Teilnehmern, die in einem Video- oder Audioanruf aus dem Chat zulässig sind, beträgt 20. Anrufe sind nicht identisch mit Audiokonferenzen. Audiokonferenzen (auch als Einwahl oder Einwahl bezeichnet) im Kontext einer Besprechung ermöglichen bis zu 1.000 Telefonteilnehmer.

Ausführliche Informationen finden Sie unter [Grenzwerte und Spezifikationen für Microsoft Teams](https://docs.microsoft.com/microsoftteams/limits-specifications-teams#meetings-and-calls).
