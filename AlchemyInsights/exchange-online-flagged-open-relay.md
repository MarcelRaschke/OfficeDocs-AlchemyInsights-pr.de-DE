---
title: Exchange Online fälschlicherweise als mögliches offenes Relay gekennzeichnet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "16386"
ms.date: 01/21/2022
ms.openlocfilehash: 282fda342bd8b904c6ed26f1a8509e1af7fd9f76
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63247733"
---
# <a name="exchange-online-incorrectly-flagged-as-possible-open-relay"></a>Exchange Online fälschlicherweise als mögliches offenes Relay gekennzeichnet

Office 365 verzögert die Ablehnung eines nicht autorisierten Relays bis zum Ende der Daten anstatt unmittelbar nach dem RCPT TO-Befehl in der SMTP-Unterhaltung. Dies kann dazu führen, dass einige Drittanbietertools Office 365 fälschlicherweise als potenzielles offenes Relay kennzeichnen. Dies ist jedoch NICHT standardmäßig der Fall.

Es gibt autorisierte Möglichkeiten, E-Mail-Relay über Ihren Mandanten zu konfigurieren. Weitere Informationen finden Sie unter FAQ Nr. 2 im Blogbeitrag [Office 365 Message Attribution](https://techcommunity.microsoft.com/t5/exchange-team-blog/office-365-message-attribution/ba-p/749143).
