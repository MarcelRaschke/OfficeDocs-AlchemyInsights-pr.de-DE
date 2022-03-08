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
ms.localizationpriority: medium
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: c8cc09329e6254d1484e3115e287ebd60eb32d1b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63129126"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Zugriff verweigert, Spam-Missbrauch erkannt

In der Regel tritt diese Nachricht auf, wenn Benutzer E-Mail-Nachrichten von IP-Adressen mithilfe der anfänglichen *ONMICROSOFT.COM* Domäne senden, die neuen Mandanten in Microsoft 365 zugewiesen ist. Am einfachsten können Sie dieses Problem beheben:

1. [Fügen Sie Ihrem Mandanten eine Domäne hinzu](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Ändern Sie die primäre E-Mail-Adresse Ihrer Benutzer](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) in die neue benutzerdefinierte Domäne, die Sie soeben hinzugefügt haben.
