---
title: 618 Kalenderfreigaberichtlinie
ms.author: chrisda
author: chrisda
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3800014"
- "618"
- "899"
ms.date: 04/21/2020
ms.openlocfilehash: a03847357056f0b57a59fe7e784f3016435f29e4
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66415858"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Richtlinienfehler beim Freigeben eines Kalenders

1. Führen Sie je nach Situation eine der folgenden Aktionen aus:
    - Stellen Sie mithilfe von Remote PowerShell eine Verbindung mit Exchange Online her. Weitere Informationen finden Sie unter [Herstellen einer Verbindung mit Exchange Online mithilfe von Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Öffnen Sie auf dem lokalen Server die Exchange-Verwaltungsshell.
2. Bestimmen Sie die Freigaberichtlinie, die dem Benutzer zugewiesen ist. Führen Sie dazu den folgenden Befehl aus, und notieren Sie sich die zurückgegebene Richtlinie:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualisieren Sie die Freigaberichtlinie für den Benutzer. Gehen Sie dazu wie folgt vor:
    - Öffnen Sie das Exchange Admin Center.
    - Klicken Sie auf **"Organisation**", und doppelklicken Sie dann unter **"Individuelle Freigabe**" auf die Richtlinie, die dem Benutzer zugewiesen ist. Dies ist die Richtlinie, die in Schritt 2 zurückgegeben wurde.
    - Wählen Sie auf der Seite "Freigaberegel" die Kalenderfreigabeebene aus, die Sie zulassen möchten, unter **"Geben Sie an, welche Informationen Sie freigeben möchten**". klicken Sie auf **"Speichern"**.

Weitere Informationen finden Sie unter : [Fehler "Richtlinie lässt nicht zu, dass Berechtigungen auf dieser Ebene einem oder mehreren Empfängern erteilt werden", wenn der Benutzer versucht, den Kalender freizugeben](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
