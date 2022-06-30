---
title: Antispam - 5.7.23
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001196"
- "3156"
ms.openlocfilehash: e28cd40bd6ded57e90ce035550d057b62dc766d0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66301240"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen mit der E-Mail-Zustellung für Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einer öffentlich verfügbaren SPF- oder DNS-Eintragsprüfung im Web.

Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam erkannt und über den Pool für [die Übermittlung mit hohem Risiko](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) weitergeleitet wurde. Nachrichten im Pool für die Zustellung mit hohem Risiko bestehen keine SPF-Prüfungen und werden daher von der Ziel-E-Mail-Organisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des E-Mail-Hosts wenden, an den Sie E-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Unzustellbarkeitsnachricht verfügbar ist. Der Microsoft-Support kann möglicherweise nicht weiter helfen.
