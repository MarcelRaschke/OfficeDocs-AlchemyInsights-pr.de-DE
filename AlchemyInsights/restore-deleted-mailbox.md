---
title: Wiederherstellen des gelöschten Postfachs
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.localizationpriority: medium
ms.custom:
- "3500005"
- "360"
search.appverid:
- MOE150
- MED150
- MBS150
ms.openlocfilehash: 65ad13ec38529231446de239ff3d96101a4927f8
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63232791"
---
# <a name="restore-a-deleted-mailbox"></a>Wiederherstellen eines gelöschten Postfachs

Wenn ein Benutzer eine Exchange Online Lizenz verliert, wird sein Postfach 30 Tage lang aufbewahrt und kann wiederhergestellt werden, indem dem Benutzer einfach die Lizenz erneut zugewiesen wird.
  
1. Wechseln Sie im Microsoft 365 Admin Center zur Seite "**Aktive Benutzer** \> **" des Benutzers**. Wählen Sie den betreffenden Benutzer aus.
2. Weisen Sie auf der Registerkarte **"Lizenzen und Apps**" die Exchange Online Lizenz zu, und wählen Sie **"Änderungen speichern" aus**.

Wenn Sie versuchen, ein freigegebenes Postfach oder einen benutzer, der gelöscht wurde, wiederherzustellen, kann es auch 30 Tage lang wiederhergestellt werden. Sie finden sie unter **"Benutzer** \> **gelöschte Benutzer"**. Für freigegebene Postfächer ist keine Lizenz erforderlich. Weitere Informationen finden Sie unter ["Wiederherstellen eines Benutzers"](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Die Wiederherstellung von E-Mails aus dem Postfach des Benutzers kann von Administratoren erfolgen, indem Sie zum [Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353) wechseln.

Wenn Sie schließlich versuchen, ein inaktives Postfach wiederherzustellen, [folgen Sie den Anweisungen hier](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).
