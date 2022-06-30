---
title: Maximale Anzahl von Besprechungsteilnehmern
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003355"
- "15557"
ms.openlocfilehash: cf86ca2edeb7f9eb6e564e522bbdf9cdcc8dd8f0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66432823"
---
# <a name="maximum-number-of-meeting-participants"></a>Maximale Anzahl von Besprechungsteilnehmern

Die maximale Anzahl von Teilnehmern pro Besprechung beträgt 1.000 für die meisten Lizenzen (A1-Lizenzen lassen nur 300 Teilnehmer zu). Darüber hinaus ermöglicht die schreibgeschützte Erfahrung bis zu 10.000 Listenteilnehmern (bis zu 20.000 während des Jahrs 2021), an einer Besprechung teilzunehmen, in der der Organisator über eine Lizenz für E3/E5/A3/A5 oder Government (GCC, GCC High, DoD) verfügt.

Die schreibgeschützte Erfahrung ermöglicht es den ersten 1.000 Teilnehmern, mit der vollständigen Teams-Besprechungserfahrung von Audio, Video und Chat teilzunehmen. Benutzer, die über die ersten 1.000 und bis zu 10.000 (20.000 im Laufe des Jahrs 2021) hinausgehen, verfügen über eine schreibgeschützte Erfahrung. Die schreibgeschützte Benutzeroberfläche ist standardmäßig deaktiviert und kann mithilfe dieses Teams PowerShell-Cmdlets aktiviert werden:

`Set-CsTeamsMeetingPolicy -Identity Global -StreamingAttendeeMode Enabled`

Weitere Informationen zur reinen Ansichtserfahrung finden Sie unter ["Nur-Ansicht-Besprechungen in Teams"](https://docs.microsoft.com/microsoftteams/view-only-meeting-experience).

Die maximal zulässigen Teilnehmer in einem Video- oder Audioanruf aus dem Chat sind 20. Anrufe sind nicht identisch mit Audiokonferenzen. Audiokonferenzen (auch als Einwahl oder Einwahl bezeichnet) im Kontext einer Besprechung ermöglichen bis zu 1.000 Telefonteilnehmer.

Ausführliche Informationen finden Sie [unter Grenzwerte und Spezifikationen für Microsoft Teams](https://docs.microsoft.com/microsoftteams/limits-specifications-teams#meetings-and-calls).
