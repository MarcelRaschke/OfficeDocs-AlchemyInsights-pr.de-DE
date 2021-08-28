---
title: Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: a13eec5d0d1abccd748653e7d7d9bb999b2e3b7a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58328825"
---
# <a name="need-help-with-email-sending-limits"></a>Benötigen Sie Hilfe bei E-Mail-Sendegrenzen?

Unten finden Sie die im Dienst erzwungenen **entwurfsbedingte Sendegrenzen**. Weitere Informationen zu diesen Grenzwerten sind [hier](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits) dokumentiert.

- Um von der Zustellung unerwünschter Massennachrichten abzuschrecken, wenden wir auf **alle ausgehenden und internen Nachrichten Grenzwerte für die Empfängerrate** pro Benutzer an. In allen SKUs beträgt diese Grenze **10 000 Empfänger pro Tag**.  Kunden, die seriöse kommerzielle E-Mails versenden müssen (z. B. Kunden-Newsletter), sollten einen Drittanbieter in Anspruch nehmen, der sich auf diese Dienste spezialisiert.
    **Hinweis**: Sobald die Empfängerratengrenze erreicht ist, können Nachrichten erst wieder aus dem Postfach gesendet werden, wenn die Anzahl von Empfängern, an die in den letzten 24 Stunden Nachrichten gesendet wurden, unter den Grenzwert fällt. Der Benutzer kann bis zu diesem Zeitpunkt keine Nachrichten mehr senden.
- Die Grenze der Nachrichtenrate von **30 Nachrichten pro Minute** gilt für alle SKUs. Dadurch wird festgelegt, wie viele Nachrichten ein Benutzer innerhalb eines bestimmten Zeitraums von seinem Exchange Online-Konto aus senden kann.
- Die **maximal zulässige Anzahl von Empfängern, die in den Feldern „An:“, „Cc:“ und „Bcc:“** für eine einzelne E-Mail-Nachricht über alle SKUs hinweg zulässig ist, beträgt **1000 Empfänger**. [Hier](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228) können Sie diesen Grenzwert anpassen.
