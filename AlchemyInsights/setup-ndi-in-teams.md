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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023521"
---
# <a name="turn-on-ndi-technology"></a>Aktivieren der NDI-Technologie

Die NDI-Technologie erfordert zwei Schritte, um für einen Benutzer aktiviert zu sein:

1. Der Mandantenadministrator muss die Eigenschaft "AllowNDIStreaming" in "CsTeamsMeetingPolicy" aktivieren.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nachdem diese Änderung ausgefüllt wurde, muss der Endbenutzer die NDI®technologie für den jeweiligen Client über **Einstellungen > Berechtigungen** aktivieren.

Weitere Informationen finden Sie unter [Verwenden der NDI-Technologie in Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
