---
title: Senden als E-Mail aktivierter öffentlicher Ordner in EXO
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
- "1956"
- "3500007"
ms.openlocfilehash: c01def2d15e443aacf94c68416614ac1262ecb81
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62715345"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs-E-Mail-aktivierter öffentlicher Ordner

Im folgenden Beispiel werden dem Benutzer "Send As" Berechtigungen für den E-Mail-aktivierten öffentlichen Ordner "NewPF1" zugewiesen.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Maustaste" -AccessRights 'SendAs'

Ausführliche Informationen zu Syntax und Parametern finden Sie unter ["Senden als" oder "Senden im Auftrag von" Berechtigungen für E-Mail-aktivierte öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

