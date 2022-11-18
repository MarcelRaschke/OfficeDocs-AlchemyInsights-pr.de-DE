---
title: SMTP-Relay
ms.author: v-ftangonan
author: IpeTangonan
manager: anita.danford
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9009961"
- "17060"
ms.date: 04/26/2022
ms.openlocfilehash: ac30ceeff4268ceeec38c072a2f06eb1ec7a6a44
ms.sourcegitcommit: b6faebed3da41577a0a16993b065dce49480fa7f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/29/2022
ms.locfileid: "65127273"
---
# <a name="smtp-relay"></a>SMTP-Relay

Die Einstellungen, die für Connectors konfiguriert sind, verhindern möglicherweise, dass ein andernfalls verfügbarer Connector bei den Routingüberlegungen berücksichtigt wird. Die folgenden Einstellungen sind vorhanden:

1. Status (aktiviert oder deaktiviert)
2. Adressraum
3. Adressraumtyp
4. Adressraumkosten
5. Quellserver
6. Beschränkungen der Nachrichtengröße

**Verarbeiten von Nachrichten, die nicht weitergeleitet werden können**

Wenn kein Connector vorhanden ist, der alle Auswahlkriterien erfüllt, wird eine der folgenden Aktionen ausgeführt:

- Wenn kein passender Connector für einen SMTP-Adressraum vorhanden ist, wird der Empfänger als nicht erreichbar markiert, und die Nachricht wird an die nicht erreichbare Warteschlange weitergeleitet. Weitere Informationen zur nicht erreichbaren Warteschlange finden Sie unter [Warteschlangentypen](https://docs.microsoft.com/exchange/mail-flow/queues/queues?view=exchserver-2019#types-of-queues&preserve-view=true).
- Wenn kein passender Connector für einen Nicht-SMTP-Adressraum vorhanden ist, wird ein Unzustellbarkeitsbericht (auch NDR, Non-Delivery Report, oder Unzustellbarkeitsnachricht genannt) an den Absender zurückgegeben.
- Wenn eine Nachricht die Connectorgrößeneinschränkung für alle Connectors überschreitet, wird ein Unzustellbarkeitsbericht an den Absender zurückgegeben.

Weitere Informationen finden Sie [unter Connectorauswahl im Routing externer Nachrichten](https://docs.microsoft.com/exchange/mail-flow/mail-routing/connector-selection)

Wir sind für Sie da, wenn Sie weitere Unterstützung benötigen. Um sich **mit einem Microsoft-Spezialisten** für weitere Hilfe zu verbinden, wählen Sie einen Chat mit einem Microsoft-Spezialisten aus, und **klicken Sie unten auf "Live-Chat** ".
