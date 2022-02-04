---
title: Antispam - 5.7.23
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
  - 3156
  - 9001196
---

# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen bei der E-Mail-Zustellung für Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einer öffentlich verfügbaren SPF- oder DNS-Eintragsprüfung im Web.

Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den [Übermittlungspool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)mit hohem Risiko weitergeleitet wurde. Nachrichten im Übermittlungspool mit hohem Risiko bestehen keine SPF-Prüfungen und werden daher von der Ziel-E-Mail-Organisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des E-Mail-Hosts wenden, an den Sie E-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Unzustellbarkeitsnachricht verfügbar ist. Der Microsoft-Support kann möglicherweise nicht weiter helfen.
