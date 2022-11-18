---
title: Aktivieren der NDI-Technologie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: a7e1f4b2f549fbfba8cbf150fab081783c7d1ee0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66417838"
---
# <a name="turn-on-ndi-technology"></a>Aktivieren der NDI-Technologie

Die NDI-Technologie erfordert zwei Schritte, die für einen Benutzer aktiviert werden müssen:

1. Der Mandantenadministrator muss die Eigenschaft "AllowNDIStreaming" in CsTeamsMeetingPolicy aktivieren.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Nachdem diese Änderung aufgefüllt wurde, muss der Endbenutzer die NDI-Technologie® für den jeweiligen Client über **Einstellungen > Berechtigungen** aktivieren.

Weitere Informationen finden [Sie unter Verwenden der NDI-Technologie in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
