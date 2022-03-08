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
ms.localizationpriority: medium
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 3e225b3edf8f4a6c28492d9551fe9b4cef0c0e3b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63199400"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs-E-Mail-aktivierter öffentlicher Ordner

Im folgenden Beispiel werden dem Benutzer "Send As" Berechtigungen für den E-Mail-aktivierten öffentlichen Ordner "NewPF1" zugewiesen.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Doppelklick" -AccessRights 'SendAs'

Ausführliche Informationen zu Syntax und Parametern finden Sie unter ["Senden als" oder "Senden im Auftrag von" Berechtigungen für E-Mail-aktivierte öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

