---
title: Fehler beim Senden von E-Mails, die durch SpamDaten blockiert wurden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: f7059c70f5072d8eb71d10fe7b14cf1c4c95217d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63277289"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von E-Mails: Clienthost mit Spamordner blockiert

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste im Besitz von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Zu den Gründen für die Sperrung durch Spamdateien gehören kompromittierte Konten, kompromittierte Computer, die eine öffentliche IP-Adresse teilen, und Internetdienstanbieter-Richtlinien (Internet Service Provider, ISP). Mögliche Fixes sind:
  
- Für blockierte eingehende Nachrichten, in denen Sie den Quell-E-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamspeicher-Website entfernen.

- Bei blockierten eingehenden Nachrichten, bei denen die Quell-IP-Adresse einer anderen Person gehört, muss der Adressbesitzer den Block von der Spamspeicher-Website entfernen. Wenn die IP-Adresse in der Richtliniensperrliste (Policy Block List, PBL) enthalten ist, kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus der PBL entfernen.

- Für blockierte ausgehende Nachrichten aus Ihrer Domäne, die mit Microsoft verbunden sind, können Sie diesen Fehler erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden. Sie können ein WHOIS-Suchtool verwenden, um den blockierten IP-Adressbesitzer zu finden.
