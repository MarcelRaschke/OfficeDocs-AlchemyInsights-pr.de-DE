---
title: Gelöschtes Postfach wiederherstellen
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500005"
- "360"
search.appverid:
- MOE150
- MED150
- MBS150
ms.openlocfilehash: c5d991ea6e87d00c1cabb7ec9c9227ffe9b95925
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66513084"
---
# <a name="restore-a-deleted-mailbox"></a>Wiederherstellen eines gelöschten Postfachs

Wenn ein Benutzer eine Exchange Online Lizenz verliert, wird sein Postfach 30 Tage lang aufbewahrt und kann wiederhergestellt werden, indem die Lizenz dem Benutzer einfach erneut zugewiesen wird.
  
1. Wechseln Sie in der Microsoft 365 Admin Center zur Seite "[**Aktive Benutzer**](https://admin.microsoft.com/AdminPortal/Home?ref=users)\>". Wählen Sie den betreffenden Benutzer aus.
2. Weisen Sie auf der Registerkarte **"Lizenzen und Apps**" die Exchange Online Lizenz zu, und wählen Sie **"Änderungen speichern"** aus.

Wenn Sie versuchen, ein freigegebenes Postfach oder einen gelöschten Benutzer wiederherzustellen, kann es auch 30 Tage lang wiederhergestellt werden. Sie finden sie unter **"Benutzer** \> **gelöschte Benutzer"**. Für freigegebene Postfächer ist keine Lizenz erforderlich. Siehe [Wiederherstellen eines Benutzers](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Die Wiederherstellung von E-Mails aus dem Postfach des Benutzers kann von Administratoren über das [Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353) erfolgen.

Wenn Sie schließlich versuchen, ein inaktives Postfach wiederherzustellen, [folgen Sie den Anweisungen hier](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).
