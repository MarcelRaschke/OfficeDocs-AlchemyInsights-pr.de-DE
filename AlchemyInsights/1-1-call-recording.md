---
title: 1:1-Anrufaufzeichnung
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
ms.openlocfilehash: 5f12715a1cc444049995cf6b0295da1ff2574ceb
ms.sourcegitcommit: a4f442784dc5c3141dbb381c6e0e700f2f6cfb6a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63386510"
---
# <a name="11-call-recording"></a>1:1-Anrufaufzeichnung

Wenn die Schaltfläche **"Aufzeichnung starten** " in einem 1:1-Anruf ausgegraut ist, ändern Sie die Richtlinieneinstellungen für den betroffenen Benutzer. Führen Sie zum Überprüfen der Richtlinieneinstellung **[Tests aus: Teams 1:1-Anrufaufzeichnung](https://aka.ms/Teams11CallRecDiag)**.

Am 31. Mai 2021 haben wir damit begonnen, eine neue Teams Calling  *PolicyAllowCloudRecordingForCalls* zu erzwingen. Vor dieser Änderung wurde die Aufzeichnung von 1:1-Anrufen durch die *AllowCloudRecording* Teams Besprechungsrichtlinie gesteuert. Diese Änderung ist in der [Einführung der Richtlinie "1:1 Anrufaufzeichnung"](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) im Nachrichtencenter -Beitrag (aktualisiert) dokumentiert.  

Standardmäßig ist die `AllowCloudRecordingForCalls` Anrufrichtlinienoption auf `$False`. Wenn Sie die Aufzeichnung von 1:1-Anrufen für alle Benutzer blockieren möchten, müssen Sie keine Maßnahmen ergreifen.

Um die Aufzeichnung von Anrufen für alle Benutzer in 1:1-Anrufen zuzulassen, verwenden  [Sie Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install), um das folgende Cmdlet auszuführen:

```PowerShell
Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True
```

Alternativ können Sie eine neue Richtlinie erstellen und `-AllowCloudRecordingForCalls` `$true` diese Richtlinie festlegen und Ihren Benutzern zuweisen.

Weitere Informationen finden Sie unter ["1:1 Richtliniensteuerungen für die Aufzeichnung von Anrufen" (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
