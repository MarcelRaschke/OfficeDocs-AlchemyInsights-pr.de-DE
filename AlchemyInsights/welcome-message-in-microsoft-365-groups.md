---
title: Begrüßungsnachricht in Microsoft 365-Gruppen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: 9e16f52333e431e48cb654e5e368572849323f28
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63196016"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Begrüßungsnachricht in Microsoft 365-Gruppen

Neue Benutzer, die einer Microsoft 365-Gruppe beitreten, erhalten eine Begrüßungs-E-Mail, wenn die Eigenschaft „UnifiedGroupWelcomeMessageEnabled“ auf „true“ gesetzt ist.

Für den Fall, dass Sie die Begrüßungsnachricht deaktivieren möchten, verwenden Sie folgenden [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)-Befehl:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
