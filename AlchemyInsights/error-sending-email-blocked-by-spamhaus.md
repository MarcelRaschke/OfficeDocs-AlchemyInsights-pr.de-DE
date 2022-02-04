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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 6d86c63cf9c6fa731ba49155408334e4a30e04b5
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61938307"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von E-Mails: Clienthost mit Spamordner blockiert

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste, die [Spam eigen](https://go.microsoft.com/fwlink/p/?linkid=123245)ist. Zu den Gründen für die Sperrung durch Spamdateien gehören kompromittierte Konten, kompromittierte Computer, die eine öffentliche IP-Adresse teilen, und Internetdienstanbieter-Richtlinien (Internet Service Provider, ISP). Mögliche Fixes sind:
  
- Für blockierte eingehende Nachrichten, in denen Sie den Quell-E-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamspeicher-Website entfernen.

- Bei blockierten eingehenden Nachrichten, bei denen die Quell-IP-Adresse einer anderen Person gehört, muss der Adressbesitzer den Block von der Spamspeicher-Website entfernen. Wenn die IP-Adresse in der Richtliniensperrliste (Policy Block List, PBL) enthalten ist, kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus der PBL entfernen.

- Für blockierte ausgehende Nachrichten aus Ihrer Domäne, die mit Microsoft verbunden sind, können Sie diesen Fehler erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden. Sie können ein WHOIS-Suchtool verwenden, um den blockierten IP-Adressbesitzer zu finden.
