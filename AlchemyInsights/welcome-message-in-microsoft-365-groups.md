---
title: Begrüßungsnachricht in Microsoft 365-Gruppen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: ee3eb54e84675efa0cb88fc43bd0cf9a6743a355
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66527880"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Begrüßungsnachricht in Microsoft 365-Gruppen

Neue Benutzer, die einer Microsoft 365-Gruppe beitreten, erhalten eine Begrüßungs-E-Mail, wenn die Eigenschaft „UnifiedGroupWelcomeMessageEnabled“ auf „true“ gesetzt ist.

Für den Fall, dass Sie die Begrüßungsnachricht deaktivieren möchten, verwenden Sie folgenden [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)-Befehl:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
