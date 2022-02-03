---
title: Problembehandlung bei Ereignissen aus E-Mails
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 04383cf9ad7a792bf0e9dbbec4caa85ec8ab7c64
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61946590"
---
# <a name="troubleshooting-events-from-email"></a>Problembehandlung bei Ereignissen aus E-Mails

1. Überprüfen Sie, ob das Feature für das Postfach aktiviert ist: **Get-EventsFromEmailConfiguration -Identity \<mailbox\>**

2. Dann schauen Sie sich die "Ereignisse aus E-Mails"-Protokollen an: **Export-MailboxDiagnosticLogs \<mailbox\> -Component TimeProfile**

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