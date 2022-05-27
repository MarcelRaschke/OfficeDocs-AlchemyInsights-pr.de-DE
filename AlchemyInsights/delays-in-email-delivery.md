---
title: Verzögerungen bei der Zustellung von E-Mail-Nachrichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100012"
- "16960"
ms.date: 03/31/2022
ms.openlocfilehash: 98a476a3837415b3efec7289e23a3c0d6a182e4e
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65709285"
---
# <a name="delays-in-email-message-delivery"></a>Verzögerungen bei der Zustellung von E-Mail-Nachrichten

Es sieht so aus, als hätten Sie ein Problem mit dem Nachrichtenfluss. Diese Diagnose kann dazu beitragen, viele häufige Probleme mit dem Nachrichtenfluss zu identifizieren:

- Überprüfen Sie die DNS-Einträge, insbesondere MX. Ein falscher MX-Eintrag kann ein Routingproblem oder zeitweilige Verzögerungen verursachen. Führen Sie den [DNS-Konnektivitätstest aus](https://testconnectivity.microsoft.com/tests/O365ExchangeDns/input).
- Wenn keine DNS-bezogenen Probleme vorhanden sind, können Nachrichtenkopfzeilen hilfreich sein, um den Hop zu ermitteln, in dem die Verzögerung aufgetreten ist. Informationen zum Analysieren der Nachrichtenkopfzeilen finden Sie unter [Nachrichtenkopfanalyse](https://aka.ms/headeranalyzer).
- Wenn Sie E-Mails über ProofPoint oder andere SendMail-Messagingsysteme weiterleiten und Verzögerungen beim Senden von E-Mails an Exchange Online auftreten, lesen [Sie "Konfigurieren von Proofpoint-E-Mail-Schutz mit Exchange Online](https://docs.microsoft.com/exchange/troubleshoot/email-delivery/configure-proofpoint-with-exchange)".
- Wenn das Problem in Outlook Web App nicht auftritt, handelt es sich wahrscheinlich um ein Clientproblem. Versuchen Sie, das Profil neu zu erstellen.  
- Um nach Problemen mit verzögerten E-Mails zu suchen, können Sie die [Nachrichtenablaufverfolgung](https://admin.exchange.microsoft.com/#/messagetrace) ausführen.  
- Führen Sie bei Verzögerungen bei eingehenden E-Mails den [Test für eingehende SMTP-E-Mails aus](https://testconnectivity.microsoft.com/tests/O365InboundSmtp/input). Führen Sie bei Problemen im Zusammenhang mit ausgehenden E-Mails den [Test für ausgehende SMTP-E-Mails](https://testconnectivity.microsoft.com/tests/O365OutboundSmtp/input) aus.
