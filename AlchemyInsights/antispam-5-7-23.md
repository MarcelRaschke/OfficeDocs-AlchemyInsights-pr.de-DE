---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932168"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen bei der E-Mail-Zustellung für Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einer öffentlich verfügbaren SPF- oder DNS-Eintragsprüfung im Web.

Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den [Übermittlungspool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)mit hohem Risiko weitergeleitet wurde. Nachrichten im Übermittlungspool mit hohem Risiko bestehen keine SPF-Prüfungen und werden daher von der E-Mail-Zielorganisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des E-Mail-Hosts wenden, an den Sie E-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Unzustellbarkeitsnachricht verfügbar ist. Der Microsoft-Support kann möglicherweise nicht weiter helfen.
