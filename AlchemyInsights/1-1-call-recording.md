---
title: 1:1 Anrufaufzeichnung
author: v-smandalika
ms.author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002530"
- "7648"
ms.date: 03/08/2022
ms.openlocfilehash: 836552024c64e35650f71f89df86185b4051eec0
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65718153"
---
# <a name="11-call-recording"></a>1:1 Anrufaufzeichnung

Wenn die Schaltfläche " **Aufzeichnung starten** " in einem 1:1-Anruf abgeblendet ist, ändern Sie die Richtlinieneinstellungen für den betroffenen Benutzer. Um die Richtlinieneinstellung zu überprüfen, **[führen Sie Tests aus: Teams 1:1-Anrufaufzeichnung](https://aka.ms/Teams11CallRecDiag)**.

Am 31. Mai 2021 haben wir begonnen, eine neue Teams Anrufrichtlinie *AllowCloudRecordingForCalls* zu erzwingen. Vor dieser Änderung wurde die Aufzeichnung von 1:1-Anrufen durch die *AllowCloudRecording-Teams-Besprechungsrichtlinie* gesteuert. Diese Änderung ist in der Einführung der Richtlinie für die Anrufaufzeichnung im Nachrichtencenterbeitrag [(aktualisiert) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) dokumentiert.  

Standardmäßig ist die `AllowCloudRecordingForCalls` Anrufrichtlinienoption auf `$False`. Wenn Sie es vorziehen, alle Benutzer an der Aufzeichnung von 1:1-Anrufen zu hindern, müssen Sie keine Maßnahmen ergreifen.

Verwenden Sie [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install), um die Anrufaufzeichnung für alle Benutzer in 1:1-Anrufen zuzulassen, um das folgende Cmdlet auszuführen:

```PowerShell
Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True
```

Alternativ können Sie eine neue Richtlinie erstellen und diese Richtlinie ihren Benutzern festlegen `-AllowCloudRecordingForCalls` `$true` und diesen zuweisen.

Weitere Informationen finden Sie unter [1:1 Richtliniensteuerelemente für Die Anrufaufzeichnung sind (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
