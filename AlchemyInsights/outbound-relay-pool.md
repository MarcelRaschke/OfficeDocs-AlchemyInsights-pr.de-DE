---
title: Ausgehender Relaypool
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
- "12315"
ms.date: 07/08/2021
ms.openlocfilehash: 9981a841b97b0b77d877e1497b4cb23edfc1e49c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66349707"
---
# <a name="outbound-relay-pool"></a>Ausgehender Relaypool

Microsoft nimmt einige Änderungen an der Konfiguration für das Weiterleiten oder Weiterleiten von E-Mails über Microsoft 365 vor. Nachrichten in bestimmten Szenarien werden über Microsoft 365 mithilfe eines speziellen Relaypools weitergeleitet oder weitergeleitet. Nachrichten, die mithilfe des Relaypools gesendet werden, könnten im Junk-E-Mail-Ordner des Empfängers landen. Weitere Informationen finden Sie unter ["Pools für ausgehende Übermittlung"](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Um ein Szenario mithilfe des Relaypools zu vermeiden, stellen Sie sicher, dass weitergeleitete/weitergeleitete Nachrichten eines der folgenden Kriterien erfüllen:

- Der ausgehende Absender ist eine akzeptierte Domäne des Mandanten.
- Sender Policy Framework (SPF) wird übergeben, wenn die Nachricht an Microsoft 365 kommt.
- DomainKeys Identified Mail (DKIM) in der Domäne des P2-Absenders wird übergeben, wenn die Nachricht an Microsoft 365 übermittelt wird.
 
Nachrichten, die den oben genannten Kriterien entsprechen, werden nicht über den Relaypool weitergeleitet.

Wenn der MX-Eintrag für Ihre Domäne auf einen Drittanbieter oder einen lokalen Server verweist, verwenden Sie erweiterte Filterung, um sicherzustellen, dass die SPF-Überprüfung für eingehende E-Mails korrekt ist, und um das Senden von E-Mails über den Relaypool zu vermeiden.

**Wie können wir feststellen, ob wir vom Relaypool betroffen sind?**

Wenn Ihre weitergeleiteten oder weitergeleiteten E-Mails eines der oben genannten Kriterien verwenden, werden Nachrichten nicht über den Relaypool weitergeleitet. Wenn eine Nachricht jedoch über einen Relaypool gesendet wird, befindet sich die ip-Adresse des ausgehenden Servers im Bereich 40.95.0.0/16, und der Name des ausgehenden Servers enthält **Rly** im Namen.

