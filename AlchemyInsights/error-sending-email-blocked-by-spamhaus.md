---
title: Fehler beim Senden von E-Mails, die von SpamHaus blockiert wurden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100003"
- "255"
ms.date: 04/21/2020
ms.openlocfilehash: 3bba3202f80972fc52938a0eb628f6de1867d2fd
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66435208"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von E-Mails: Clienthost mit Spamhaus blockiert

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Gründe für die Blockierung durch Spamhaus sind kompromittierte Konten, kompromittierte Computer, die eine öffentliche IP-Adresse teilen, und Internetdienstanbieterrichtlinien (Internet Service Provider, ISP). Mögliche Korrekturen sind:
  
- Für blockierte eingehende Nachrichten, bei denen Sie den Quell-E-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamhaus-Website entfernen.

- Bei blockierten eingehenden Nachrichten, bei denen die Quell-IP-Adresse einer anderen Person gehört, muss der Adressbesitzer den Block von der Spamhaus-Website entfernen. Wenn sich die IP-Adresse in der Richtlinienblockliste (Policy Block List, PBL) befindet, kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus der PBL entfernen.

- Bei blockierten ausgehenden Nachrichten aus Ihrer Domäne, die mit Microsoft verbunden sind, können Sie diese Fehlermeldung erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden. Sie können ein WHOIS-Nachschlagetool verwenden, um den Besitzer der blockierten IP-Adresse zu finden.
