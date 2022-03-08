---
title: Optionen für den weitergeleiteten Besprechungsbeitritt
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
- "9002255"
- "15518"
ms.openlocfilehash: 92c0b1a312d2f4f93439f2ec640642e96df81a1b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63172327"
---
# <a name="forwarded-meeting-join-options"></a>Optionen für den weitergeleiteten Besprechungsbeitritt

Wenn Sie eine Teams Besprechung an ein Teams Besprechungsraum Gerät weitergeleitet haben und die Schaltfläche zum Beitreten fehlt, gehen Sie wie folgt vor:

1. Stellen Sie sicher, dass das Besprechungsraum-Konto so festgelegt ist, dass Buchungsanfragen automatisch akzeptiert werden.
1. Legen Sie drei Parameter über PowerShell fest (Exchange Online oder Exchange lokal, je nach Umgebungskonfiguration):
    - ProcessExternalMeetingMessages $true
    - DeleteComments $false
    - DeleteSubject-$false

Weitere Informationen finden Sie unter ["Set-CalendarProcessing"](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-calendarprocessing?view=exchange-ps&preserve-view=true)

Beispiel: `Set-CalendarProcessing -Identity [UPN] -ProcessExternalMeetingMessages $true -DeleteComments $false -DeleteSubject $false`

**Hinweis**: Dieses Problem wird am häufigsten durch eine falsche Konfiguration eines Besprechungsraum Postfachs für Besprechungen von Drittanbietern oder lokale Hybridumgebungen Exchange verursacht.

Weitere Informationen zum Teilnehmen an Besprechungen von Drittanbietern über einen Microsoft Teams Raum finden Sie unter [Aktivieren Teams Raumgeräte für die Teilnahme an Besprechungen von Drittanbietern](https://docs.microsoft.com/microsoftteams/rooms/third-party-join#step-1-allow-calendar-invite-processing-for-third-party-meetings).

Weitere Informationen zum Bereitstellen von Microsoft Teams-Räume mit Exchange lokalen Bereitstellungen finden Sie unter ["Bereitstellen von Microsoft Teams-Räume mit Exchange lokal"](https://docs.microsoft.com/microsoftteams/rooms/with-exchange-on-premises).
