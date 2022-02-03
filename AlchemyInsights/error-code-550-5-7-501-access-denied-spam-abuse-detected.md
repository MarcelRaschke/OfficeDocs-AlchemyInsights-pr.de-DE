---
title: Fehlercode 550 5.7.501 Zugriff verweigert, Spam-Missbrauch erkannt
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: f56511c4d1ffc7e81269fb769c2e8cd74d40abf9
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61961854"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Zugriff verweigert, Spam-Missbrauch erkannt

In der Regel tritt diese Nachricht auf, wenn Benutzer E-Mail-Nachrichten von IP-Adressen mithilfe der anfänglichen *ONMICROSOFT.COM* Domäne senden, die neuen Mandanten in Microsoft 365 zugewiesen ist. Am einfachsten können Sie dieses Problem beheben:

1. [Fügen Sie Ihrem Mandanten eine Domäne hinzu.](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)

2. [Ändern Sie die primäre E-Mail-Adresse Ihrer Benutzer](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) in die neue benutzerdefinierte Domäne, die Sie soeben hinzugefügt haben.
