---
title: Blockieren der Aufzeichnung von Besprechungen durch Benutzer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 53ca3dee5a18b81873cfe3d4398303baa411e5ca
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63175027"
---
# <a name="block-user-from-recording-meetings"></a>Blockieren der Aufzeichnung von Besprechungen durch Benutzer

Wenn Sie **verhindern oder blockieren** müssen, dass bestimmte Benutzer Teams Besprechungen aufzeichnen, können Sie dies über Teams Besprechungsrichtlinieneinstellungen tun. Deaktivieren Sie im Microsoft Teams Admin Center die Einstellung "**Cloudaufzeichnung zulassen**" in der Besprechungsrichtlinie, die diesem Benutzer zugewiesen ist. Weitere Informationen finden Sie unter [Verwalten von Besprechungsrichtlinien in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Verwenden Sie die Supportdiagnose, um zu überprüfen, ob ein bestimmter Benutzer Teams Besprechungen aufzeichnen darf oder nicht. Führen Sie eine neue Supportabfrage und einen neuen Typ in **Diag: Besprechungsaufzeichnung** aus– die Diagnose überprüft die Richtlinieneinstellungen für den angegebenen Benutzer und ermittelt deren Richtlinieneinstellungen. Denken Sie daran, dass es einige Stunden dauern kann, bis neue Richtlinieneinstellungen wirksam werden. Wenn Sie also gerade eine Änderung vorgenommen haben, warten Sie einige Stunden, bevor Sie die Diagnose erneut ausführen.

Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren der Cloudaufzeichnung](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).
