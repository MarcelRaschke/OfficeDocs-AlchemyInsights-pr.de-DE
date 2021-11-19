---
title: Optionen für den weitergeleiteten Besprechungsbeitritt
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
- "9002255"
- "15518"
ms.openlocfilehash: 4be78ddd183cc731165d04337a74db56e6909cf4
ms.sourcegitcommit: f68d9a8ff938cb2defddc8f24954e88056481b4d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/18/2021
ms.locfileid: "61079246"
---
# <a name="forwarded-meeting-join-options"></a>Optionen für den weitergeleiteten Besprechungsbeitritt

Wenn Sie eine Teams Besprechung an ein Teams Besprechungsraum Gerät weitergeleitet haben und die Schaltfläche "Beitreten" fehlt, gehen Sie wie folgt vor:

1. Stellen Sie sicher, dass das Besprechungsraum-Konto so festgelegt ist, dass Buchungsanfragen automatisch akzeptiert werden.
1. Legen Sie drei Parameter über PowerShell fest (Exchange Online oder Exchange lokal, je nach Umgebungskonfiguration):
    - ProcessExternalMeetingMessages $true
    - DeleteComments $false
    - DeleteSubject-$false

Weitere Informationen finden Sie unter ["Set-CalendarProcessing"](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-calendarprocessing?view=exchange-ps&preserve-view=true)

Beispiel: `Set-CalendarProcessing -Identity [UPN] -ProcessExternalMeetingMessages $true -DeleteComments $false -DeleteSubject $false`

**Hinweis:** Dieses Problem wird am häufigsten durch eine falsche Konfiguration eines Besprechungsraum Postfachs für Besprechungen von Drittanbietern oder lokale Hybridumgebungen Exchange verursacht.

Weitere Informationen zum Teilnehmen an Besprechungen von Drittanbietern über einen Microsoft Teams Raum finden Sie unter Aktivieren Teams Raumgeräte für die [Teilnahme an Besprechungen von Drittanbietern.](https://docs.microsoft.com/microsoftteams/rooms/third-party-join#step-1-allow-calendar-invite-processing-for-third-party-meetings)

Weitere Informationen zum Bereitstellen von Microsoft Teams-Räume mit Exchange lokalen Bereitstellungen finden Sie unter [Deploy Microsoft Teams-Räume with Exchange on premises.](https://docs.microsoft.com/microsoftteams/rooms/with-exchange-on-premises)
