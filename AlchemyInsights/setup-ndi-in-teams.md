---
title: Aktivieren der NDI-Technologie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: 986e5d99daa3f35710573f4f1811b3b5b232ee2f
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63084322"
---
# <a name="turn-on-ndi-technology"></a>Aktivieren der NDI-Technologie

Die NDI-Technologie erfordert zwei Schritte, um für einen Benutzer aktiviert zu sein:

1. Der Mandantenadministrator muss die Eigenschaft "AllowNDIStreaming" in "CsTeamsMeetingPolicy" aktivieren.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nachdem diese Änderung ausgefüllt wurde, muss der Endbenutzer die NDI-Technologie® für den jeweiligen Client über **Einstellungen > Berechtigungen** aktivieren.

Weitere Informationen finden Sie unter [Verwenden der NDI-Technologie in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
