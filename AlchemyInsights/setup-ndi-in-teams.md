---
title: Aktivieren der NDI-Technologie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: 265563ad8ca670fe587bab8f3f3f25030962ac35
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62727513"
---
# <a name="turn-on-ndi-technology"></a>Aktivieren der NDI-Technologie

Die NDI-Technologie erfordert zwei Schritte, um für einen Benutzer aktiviert zu sein:

1. Der Mandantenadministrator muss die Eigenschaft "AllowNDIStreaming" in "CsTeamsMeetingPolicy" aktivieren.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nachdem diese Änderung ausgefüllt wurde, muss der Endbenutzer die NDI-Technologie® für den jeweiligen Client über **Einstellungen > Berechtigungen** aktivieren.

Weitere Informationen finden Sie unter [Verwenden der NDI-Technologie in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
