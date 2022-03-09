---
title: Blockieren der Aufzeichnung von Besprechungen durch Benutzer
author: v-jmathew
ms.author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002530"
- "9325"
ms.date: 03/08/2022
ms.openlocfilehash: f968ea11a8f340937a0af1832031a5bf4e2ed98f
ms.sourcegitcommit: a4f442784dc5c3141dbb381c6e0e700f2f6cfb6a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63386445"
---
# <a name="block-user-from-recording-meetings"></a>Blockieren der Aufzeichnung von Besprechungen durch Benutzer

Wenn Sie verhindern möchten, dass bestimmte Benutzer Teams Besprechungen aufzeichnen, können Sie dies über Teams Besprechungsrichtlinieneinstellungen tun. Deaktivieren Sie im Microsoft Teams Admin Center die Einstellung "**Cloudaufzeichnung zulassen**" in der Besprechungsrichtlinie, die diesem Benutzer zugewiesen ist. Weitere Informationen finden Sie unter [Verwalten von Besprechungsrichtlinien in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Um zu überprüfen, ob ein bestimmter Benutzer Teams Besprechungen aufzeichnen darf, **[führen Sie Tests aus: Besprechungsaufzeichnung](https://aka.ms/MeetingRecordingDiag)**. Die Diagnose überprüft die Richtlinieneinstellungen für den angegebenen Benutzer und bestimmt deren Richtlinieneinstellungen. Denken Sie daran, dass es einige Stunden dauern kann, bis neue Richtlinieneinstellungen wirksam werden. Wenn Sie also gerade eine Änderung vorgenommen haben, warten Sie einige Stunden, bevor Sie die Diagnose erneut ausführen.

Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren der Cloudaufzeichnung](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).
