---
title: Exchange Online fälschlicherweise als mögliches offenes Relay gekennzeichnet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "16386"
ms.date: 01/21/2022
ms.openlocfilehash: 841b16280c4bd6cb50e8ac13244b10ace5bd4dcf
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62710665"
---
# <a name="exchange-online-incorrectly-flagged-as-possible-open-relay"></a>Exchange Online fälschlicherweise als mögliches offenes Relay gekennzeichnet

Office 365 verzögert die Ablehnung eines nicht autorisierten Relays bis zum Ende der Daten anstatt unmittelbar nach dem RCPT TO-Befehl in der SMTP-Unterhaltung. Dies kann dazu führen, dass einige Drittanbietertools Office 365 fälschlicherweise als potenzielles offenes Relay kennzeichnen. Dies ist jedoch NICHT standardmäßig der Fall.

Es gibt autorisierte Möglichkeiten, E-Mail-Relay über Ihren Mandanten zu konfigurieren. Weitere Informationen finden Sie unter FAQ Nr. 2 im Blogbeitrag [Office 365 Message Attribution](https://techcommunity.microsoft.com/t5/exchange-team-blog/office-365-message-attribution/ba-p/749143).
