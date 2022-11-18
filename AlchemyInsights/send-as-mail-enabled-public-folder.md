---
title: Als E-Mail aktivierter öffentlicher Ordner in EXO
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "1956"
ms.date: 04/21/2020
ms.openlocfilehash: fb39d365a297ecc31f1ee733ee54d2b44c2e9793
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66418018"
---
# <a name="sendas-mail-enabled-public-folder"></a>Öffentlicher Ordner "SendAs Mail enabled"

Im folgenden Beispiel werden dem Benutzer Jason "Send As"-Berechtigungen für den E-Mail-aktivierten öffentlichen Ordner NewPF1 zugewiesen.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Ausführliche Informationen zu Syntax und Parametern finden [Sie unter "Senden als"- oder "Senden im Auftrag"-Berechtigungen für E-Mail-aktivierte öffentliche Ordner](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

