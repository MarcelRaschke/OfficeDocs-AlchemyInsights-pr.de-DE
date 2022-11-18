---
title: Ordner "Ausgehende E-Mails an Junk-E-Mail"
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "2697"
ms.date: 04/21/2020
ms.openlocfilehash: 764728e91a5dcd08781b1b3865b88c982a0a3ad7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66294454"
---
# <a name="outbound-email-to-junk-email-folder"></a>Ordner "Ausgehende E-Mails an Junk-E-Mail"

Wenn ausgehende Nachrichten als Junk-E-Mail gekennzeichnet werden, führen Sie die folgenden Schritte aus:

- Falls noch nicht geschehen, sollten Sie die [Konfiguration ausgehender Spamrichtlinienbenachrichtigungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) in Betracht ziehen.

- Verwenden Sie die [Nachrichtenablaufverfolgung](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) , um festzustellen, ob die ausgehende Nachricht den Ereigniswert **"Spam** " mit dem zusätzlichen Detail aufweist: **Verwenden Sie den Übermittlungspool mit hohem Risiko**.

  Überprüfen Sie für diese Nachrichten den Nachrichteninhalt, um zu sehen, was als Spam angesehen werden könnte. Beispielsweise können Signaturen für viele Benutzer manchmal Probleme verursachen.

  Wenn Sie mehrere Beispiele für legitime ausgehende Nachrichten haben, die als Junk-E-Mail gekennzeichnet werden, öffnen Sie ein Supportticket, und bitten Sie den Supportmitarbeiter, Ihre Nachrichten als falsch positive Ergebnisse an unsere Spamanalysten zu übermitteln. Stellen Sie Beispielnachrichten bereit, die alle Nachrichtenkopfzeilen enthalten.
