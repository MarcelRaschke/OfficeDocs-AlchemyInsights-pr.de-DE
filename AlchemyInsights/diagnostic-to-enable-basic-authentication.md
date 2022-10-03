---
title: Diagnose zum Aktivieren der Standardauthentifizierung für Exchange Online-Protokolle
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9006699"
- "11392"
- "17492"
ms.date: 05/27/2021
ms.openlocfilehash: 79f008fab1926f265b34c7ad2f902aad5b87462c
ms.sourcegitcommit: fd40ab0f1a1d678e25c5165e8f4612919d72e9b5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/03/2022
ms.locfileid: "68325822"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a>Diagnose zum Aktivieren der Standardauthentifizierung für Exchange Online-Protokolle

Microsoft hat diese Diagnose möglicherweise kürzlich deaktiviert, die in der Regel verwendet wird, um die Standardauthentifizierung für Exchange Online Protokolle wie POP3, IMAP4, Exchange ActiveSync, Exchange-Webdienste, Offlineadressbuch, MAPI, RPC und Remote PowerShell zu aktivieren. 

Microsoft sendet direkte Kommunikation über das Nachrichtencenter, um Mandanten mitzuteilen, wo sie die Standardauthentifizierung in der Mandantenumgebung aufgrund mangelnder Verwendung deaktivieren. Dadurch werden Mandantenumgebungen vor damit verbundenen Sicherheitsrisiken geschützt.

Weitere Informationen finden Sie unter:

- [Einstellung der Standardauthentifizierung in Exchange Online](https://learn.microsoft.com/exchange/clients-and-mobile-in-exchange-online/deprecation-of-basic-authentication-exchange-online)
- [Standardauthentifizierungsdeprecation in Exchange Online – Update vom September 2022](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-authentication-deprecation-in-exchange-online-september/ba-p/3609437)