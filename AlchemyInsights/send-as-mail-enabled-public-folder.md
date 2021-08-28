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
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052565"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs-E-Mail-aktivierter öffentlicher Ordner

Im folgenden Beispiel werden dem Benutzer "Send As" Berechtigungen für den E-Mail-aktivierten öffentlichen Ordner "NewPF1" zugewiesen.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Maustaste" -AccessRights 'SendAs'

Ausführliche Informationen zu Syntax und Parametern finden Sie unter ["Senden als" oder "Senden im Auftrag von" Berechtigungen für E-Mail-aktivierte öffentliche Ordner.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

