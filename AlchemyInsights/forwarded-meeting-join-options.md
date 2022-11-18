---
title: Optionen für den Weitergeleiteten Besprechungsbeitritt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002255"
- "15518"
ms.openlocfilehash: 1f73191e3605af23362d3e4997427e1ca13dc72c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66269164"
---
# <a name="forwarded-meeting-join-options"></a>Optionen für den Weitergeleiteten Besprechungsbeitritt

Wenn Sie eine Teams-Besprechung an ein Gerät des Teams-Besprechungsraums weitergeleitet haben und die Schaltfläche "Teilnehmen" fehlt, gehen Sie folgendermaßen vor:

1. Stellen Sie sicher, dass das Besprechungsraumkonto so eingerichtet ist, dass Buchungsanfragen automatisch akzeptiert werden.
1. Legen Sie drei Parameter über PowerShell (Exchange Online oder lokale Exchange-Umgebungskonfiguration) fest:
    - ProcessExternalMeetingMessages $true
    - DeleteComments $false
    - DeleteSubject-$false

Weitere Informationen finden Sie unter [Set-CalendarProcessing](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-calendarprocessing?view=exchange-ps&preserve-view=true)

Beispiel: `Set-CalendarProcessing -Identity [UPN] -ProcessExternalMeetingMessages $true -DeleteComments $false -DeleteSubject $false`

**Hinweis**: Dieses Problem wird meistens durch eine falsche Konfiguration eines Besprechungsraumpostfachs für Besprechungen von Drittanbietern oder lokale Hybrid-Exchange-Umgebungen verursacht.

Weitere Informationen zum Teilnehmen an Besprechungen von Drittanbietern über einen Microsoft [Teams-Raum finden Sie unter Aktivieren von Teams-Raumgeräten für die Teilnahme an Besprechungen von Drittanbietern](https://docs.microsoft.com/microsoftteams/rooms/third-party-join#step-1-allow-calendar-invite-processing-for-third-party-meetings).

Weitere Informationen zum Bereitstellen von Microsoft Teams-Räume mit lokalem Exchange finden [Sie unter Deploy Microsoft Teams-Räume with Exchange on premises](https://docs.microsoft.com/microsoftteams/rooms/with-exchange-on-premises).
