---
title: Ausgehender Relaypool
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
  - 3000003
  - 12315
---

# <a name="outbound-relay-pool"></a>Ausgehender Relaypool

Microsoft unternimmt einige Änderungen an der Konfiguration für das Weiterleiten oder Weiterleiten von E-Mails über Microsoft 365. Nachrichten in bestimmten Szenarien werden über Microsoft 365 mithilfe eines speziellen Relaypools weitergeleitet oder weitergeleitet. Nachrichten, die mithilfe des Relaypools gesendet werden, können im Junk-E-Mail-Ordner des Empfängers enden. Weitere Informationen finden Sie unter "Pools für [ausgehende Übermittlungen"](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Um ein Szenario mithilfe des Relaypools zu vermeiden, stellen Sie sicher, dass weitergeleitete/weitergeleitete Nachrichten eines der folgenden Kriterien erfüllen:

- Der ausgehende Absender ist eine akzeptierte Domäne des Mandanten.
- Sender Policy Framework (SPF) wird übergeben, wenn die Nachricht an Microsoft 365 kommt.
- DomainKeys Identified Mail (DKIM) in der P2-Absenderdomäne wird übergeben, wenn die Nachricht zu Microsoft 365 kommt.
 
Nachrichten, die die oben genannten Kriterien erfüllen, werden nicht über den Relaypool weitergeleitet.

Wenn der MX-Eintrag für Ihre Domäne auf einen Drittanbieterserver oder einen lokalen Server verweist, verwenden Sie erweiterte Filterung, um sicherzustellen, dass die SPF-Überprüfung für eingehende E-Mails korrekt ist, und um das Senden von E-Mails über den Relaypool zu vermeiden.

**Wie können wir feststellen, ob wir vom Relaypool betroffen sind?**

Wenn Ihre weitergeleiteten oder weitergeleiteten E-Mails eines der oben genannten Kriterien verwenden, werden Nachrichten nicht über den Relaypool weitergeleitet. Wenn eine Nachricht jedoch über einen Relaypool gesendet wird, befindet sich die ip-Adresse des ausgehenden Servers im Bereich 40.95.0.0/16, und der Name des ausgehenden Servers enthält **den** Namen.

