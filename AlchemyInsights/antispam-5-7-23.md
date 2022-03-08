---
title: Antispam - 5.7.23
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8019ace1e3782aca0ef51b4241562a80c62088cc
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63188348"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Beheben von Problemen bei der E-Mail-Zustellung für Fehlercode 5.7.23

Überprüfen Sie den SPF-DNS-Eintrag für Ihre Domäne bei einer öffentlich verfügbaren SPF- oder DNS-Eintragsprüfung im Web.

Stellen Sie sicher, dass die ausgehende Nachricht von Microsoft nicht als Spam identifiziert und über den [Übermittlungspool mit hohem Risiko](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) weitergeleitet wurde. Nachrichten im Übermittlungspool mit hohem Risiko bestehen keine SPF-Prüfungen und werden daher von der Ziel-E-Mail-Organisation nicht akzeptiert.

Wenn das Problem weiterhin besteht, müssen Sie sich möglicherweise an den Administrator des E-Mail-Hosts wenden, an den Sie E-Mails senden möchten. Notieren Sie sich den detaillierten externen Fehler, der in der Unzustellbarkeitsnachricht verfügbar ist. Der Microsoft-Support kann möglicherweise nicht weiter helfen.
