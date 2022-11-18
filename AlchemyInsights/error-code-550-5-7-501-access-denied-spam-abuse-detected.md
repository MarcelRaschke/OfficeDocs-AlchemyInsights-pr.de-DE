---
title: Fehlercode 550 5.7.501 Zugriff verweigert, Spammissbrauch erkannt
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100015"
- "351"
ms.date: 04/21/2020
ms.openlocfilehash: bd8c3374c39b17d333e980eb86867cbe18b5759b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66421474"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Zugriff verweigert, Spammissbrauch erkannt

In der Regel tritt diese Meldung auf, wenn Benutzer E-Mail-Nachrichten von IP-Adressen mithilfe der ursprünglichen *.onmicrosoft.com* Domäne senden, die neuen Mandanten in Microsoft 365 zugewiesen ist. Die einfachste Möglichkeit, dieses Problem zu beheben, ist:

1. [Fügen Sie Ihrem Mandanten eine Domäne hinzu](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Ändern Sie die primäre E-Mail-Adresse Ihrer Benutzer](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) in die neue benutzerdefinierte Domäne, die Sie soeben hinzugefügt haben.
