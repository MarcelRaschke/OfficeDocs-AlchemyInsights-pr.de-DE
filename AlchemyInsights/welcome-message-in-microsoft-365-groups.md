---
title: Begrüßungsnachricht in Microsoft 365-Gruppen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: e20ab3155aaa15673eafffcfddf14ec53d02152a
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62595838"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Begrüßungsnachricht in Microsoft 365-Gruppen

Neue Benutzer, die einer Microsoft 365-Gruppe beitreten, erhalten eine Begrüßungs-E-Mail, wenn die Eigenschaft „UnifiedGroupWelcomeMessageEnabled“ auf „true“ gesetzt ist.

Für den Fall, dass Sie die Begrüßungsnachricht deaktivieren möchten, verwenden Sie folgenden [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)-Befehl:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
