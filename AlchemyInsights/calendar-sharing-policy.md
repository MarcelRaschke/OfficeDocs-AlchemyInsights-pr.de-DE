---
title: 618 Kalenderfreigaberichtlinie
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 864cbc41769f88dad8eb277571048ab3b3ab6fbb
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63250361"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Richtlinienfehler beim Freigeben eines Kalenders

1. Führen Sie je nach Situation eine der folgenden Aktionen aus:
    - Verbinden mithilfe von Remote-PowerShell zum Exchange Online. Weitere Informationen finden Sie unter [Verbinden zum Exchange Online mithilfe von Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Öffnen Sie auf dem lokalen Server die Exchange Verwaltungsshell.
2. Bestimmen Sie die Freigaberichtlinie, die dem Benutzer zugewiesen ist. Führen Sie dazu den folgenden Befehl aus, und notieren Sie sich die zurückgegebene Richtlinie:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualisieren Sie die Freigaberichtlinie für den Benutzer. Gehen Sie dazu wie folgt vor:
    - Öffnen Sie das Exchange Admin Center.
    - Klicken Sie auf **"Organisation**", und doppelklicken Sie dann unter " **Individuelle Freigabe**" auf die Richtlinie, die dem Benutzer zugewiesen ist. Dies ist die Richtlinie, die in Schritt 2 zurückgegeben wurde.
    - Wählen Sie auf der Seite "Freigaberegel" die Kalenderfreigabestufe aus, die Sie zulassen möchten, unter **"Angeben, welche Informationen Sie freigeben möchten**". klicken Sie auf **"Speichern"**.

Weitere Informationen finden Sie unter [: "Richtlinie lässt nicht zu, dass einem oder mehreren der Empfänger Berechtigungen auf dieser Ebene gewährt werden", wenn der Benutzer versucht, Kalender freizugeben](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
