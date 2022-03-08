---
title: 1:1-Anrufaufzeichnung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: d9035ab90cebfeeab28ecbb97d963a28905b3f2b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63209012"
---
# <a name="11-call-recording"></a>1:1-Anrufaufzeichnung

Wenn die Schaltfläche **"Aufzeichnung starten** " in einem 1:1-Anruf ausgegraut ist, müssen Sie die Richtlinieneinstellungen für den betroffenen Benutzer ändern. Um die Richtlinieneinstellung zu überprüfen, führen Sie die Diagnose für den betroffenen Benutzer aus, indem Sie **Diag: Teams 1:1-Anrufaufzeichnung** oben eingeben.     

Ab dem 31. Mai 2021 werden wir mit der Erzwingung einer neuen Teams  *AnrufrichtlinieAllowCloudRecordingForCalls* beginnen. Vor dieser Änderung wird die Aufzeichnung von 1:1-Anrufen durch die *AllowCloudRecording-Teams* Besprechungsrichtlinie gesteuert. Diese Änderung ist in der Einführung der Richtlinie zur Anrufaufzeichnung im Nachrichtencenter dokumentiert:  [(Aktualisiert) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*  Die Anrufrichtlinienoption ist standardmäßig auf **$False** festgelegt. Wenn Sie die Aufzeichnung von 1:1-Anrufen für alle Benutzer blockieren möchten, müssen Sie keine Maßnahmen ergreifen.  

Um die Anrufaufzeichnung für alle Benutzer in 1:1-Anrufen zu aktivieren  [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) das folgende Cmdlet ausführen: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativ können Sie eine neue Richtlinie erstellen und **"-AllowCloudRecordingForCalls** " festlegen, um diese Richtlinie zu **$true** und Ihren Benutzern zuzuweisen. 

Weitere Informationen finden Sie unter ["1:1 Richtliniensteuerungen für die Aufzeichnung von Anrufen" (fast!) Hier](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
