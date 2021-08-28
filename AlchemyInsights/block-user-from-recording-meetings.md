---
title: Blockieren der Aufzeichnung von Besprechungen durch Benutzer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019183"
---
# <a name="block-user-from-recording-meetings"></a>Blockieren der Aufzeichnung von Besprechungen durch Benutzer

Wenn Sie **verhindern oder blockieren** müssen, dass bestimmte Benutzer Teams Besprechungen aufzeichnen, können Sie dies über Teams Besprechungsrichtlinieneinstellungen tun. Deaktivieren Sie im Microsoft Teams Admin Center die Einstellung **"Cloudaufzeichnung zulassen"** in der Besprechungsrichtlinie, die diesem Benutzer zugewiesen ist. Weitere Informationen finden Sie unter [Verwalten von Besprechungsrichtlinien in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Verwenden Sie die Supportdiagnose, um zu überprüfen, ob ein bestimmter Benutzer Teams Besprechungen aufzeichnen darf oder nicht. Führen Sie eine neue Supportabfrage und einen neuen Typ in **Diag: Besprechungsaufzeichnung** aus– die Diagnose überprüft die Richtlinieneinstellungen für den angegebenen Benutzer und ermittelt deren Richtlinieneinstellungen. Denken Sie daran, dass es einige Stunden dauern kann, bis neue Richtlinieneinstellungen wirksam werden. Wenn Sie also gerade eine Änderung vorgenommen haben, warten Sie einige Stunden, bevor Sie die Diagnose erneut ausführen.

Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren der Cloudaufzeichnung.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
