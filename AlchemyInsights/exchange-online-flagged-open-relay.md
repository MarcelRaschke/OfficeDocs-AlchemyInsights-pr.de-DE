---
title: Exchange Online fälschlicherweise als mögliches offenes Relay gekennzeichnet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3000003"
- "16386"
ms.date: 01/21/2022
ms.openlocfilehash: 9cd220029092ebc94d9e8a923359b3edd8a282d2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66435064"
---
# <a name="exchange-online-incorrectly-flagged-as-possible-open-relay"></a>Exchange Online fälschlicherweise als mögliches offenes Relay gekennzeichnet

Office 365 verzögert die Ablehnung eines nicht autorisierten Relays bis nach Dem Ende der Daten anstatt unmittelbar nach dem Befehl RCPT TO in der SMTP-Unterhaltung. Dies kann dazu führen, dass einige Drittanbietertools Office 365 fälschlicherweise als potenzielles offenes Relay kennzeichnen. Dies ist jedoch nicht standardmäßig der Fall.

Es gibt autorisierte Möglichkeiten zum Konfigurieren des E-Mail-Relays über Ihren Mandanten. Weitere Informationen finden Sie unter häufig gestellte Fragen Nr. 2 im Blogbeitrag [Office 365 Nachrichtenzuordnung](https://techcommunity.microsoft.com/t5/exchange-team-blog/office-365-message-attribution/ba-p/749143).
