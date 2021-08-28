---
title: Ausgehende E-Mails im Junk-E-Mail-Ordner
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096657"
---
# <a name="outbound-email-to-junk-email-folder"></a>Ausgehende E-Mails im Junk-E-Mail-Ordner

Wenn ausgehende Nachrichten als Junk gekennzeichnet werden, führen Sie die folgenden Schritte aus:

- Falls noch nicht geschehen, sollten Sie die [Konfiguration ausgehender Spamrichtlinienbenachrichtigungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)in Betracht ziehen.

- Verwenden Sie [die Nachrichtenablaufverfolgung,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) um festzustellen, ob die ausgehende Nachricht den Ereigniswert **Spam** mit dem zusätzlichen Detail enthält: Verwenden Sie den **Übermittlungspool mit hohem Risiko.**

  Überprüfen Sie für diese Nachrichten den Nachrichteninhalt, um zu sehen, was als Spam betrachtet werden kann. Signaturen können beispielsweise für viele Benutzer manchmal Probleme verursachen.

  Wenn Sie mehrere Beispiele für seriöse ausgehende Nachrichten haben, die als Junk gekennzeichnet sind, öffnen Sie ein Supportticket, und bitten Sie den Support-Agent, Ihre Nachrichten als falsch positive Ergebnisse an unsere Spamanalysten zu übermitteln. Stellen Sie Beispielnachrichten bereit, die alle Nachrichtenkopfzeilen enthalten.
