---
title: Problembehandlung bei Ereignissen aus E-Mails
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105351"
---
# <a name="troubleshooting-events-from-email"></a>Problembehandlung bei Ereignissen aus E-Mails

1. Überprüfen Sie, ob das Feature für das Postfach aktiviert ist: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Dann schauen Sie sich die "Ereignisse aus E-Mails"-Protokollen an: **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Suchen Sie in den Protokollen "Ereignisse aus E-Mails" nach dem InternetMessageId, das dem Element im Postfach entspricht.  

4. Die TrustScore bestimmt, ob das Element hinzugefügt wird. Ereignisse werden nur hinzugefügt, wenn die TrustScore = "vertrauenswürdig" lautet.

Die TrustScore wird durch die Eigenschaften SPF, Dkim oder Dmarc bestimmt, die sich im Nachrichtenkopf befinden.

So zeigen Sie diese Eigenschaften an:

**Desktop-Outlook**

- Öffnen Sie das Element,
- Datei -> Eigenschaften -> Internet-Kopfzeilen

oder

**MFCMapi**

- Navigieren Sie zu dem Element im Posteingang
- Suchen Sie nach PR_TRANSPORT_MESSAGE_HEADERS_W

Diese Eigenschaften werden ermittelt und während des Transports und des Routings aufgezeichnet. Zur weiteren Problembehandlung müssen Sie möglicherweise die Transport Unterstützung zu den Fehlern in SPF, DKIM und/oder DMARC nachverfolgen.