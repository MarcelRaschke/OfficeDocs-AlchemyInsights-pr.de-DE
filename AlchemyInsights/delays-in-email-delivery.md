---
title: Verzögerungen bei der Zustellung von E-Mail-Nachrichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3100012"
- "16960"
ms.date: 03/31/2022
ms.openlocfilehash: b561cfcca28bbf80b0a69e4bd79337c43d58420c
ms.sourcegitcommit: 01c1bc49e5972cd4a4aec6426774d9ff0ec99ae1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2022
ms.locfileid: "64592536"
---
# <a name="delays-in-email-message-delivery"></a>Verzögerungen bei der Zustellung von E-Mail-Nachrichten

Es sieht so aus, als hätten Sie ein Problem mit dem Nachrichtenfluss. Diese Diagnose kann dabei helfen, viele häufige Probleme mit dem Nachrichtenfluss zu identifizieren:

- Überprüfen Sie die DNS-Einträge, insbesondere MX. Ein falscher MX-Eintrag kann ein Routingproblem oder eine zeitweilige Verzögerung verursachen. Führen Sie den [DNS-Konnektivitätstest aus](https://testconnectivity.microsoft.com/tests/O365ExchangeDns/input).
- Wenn keine DNS-bezogenen Probleme auftreten, können Nachrichtenheader hilfreich sein, um den Hop zu bestimmen, in dem die Verzögerung aufgetreten ist. Informationen zum Analysieren der Nachrichtenkopfzeilen finden Sie unter ["Nachrichtenkopfanalyse"](https://aka.ms/headeranalyzer).
- Wenn Sie E-Mails über ProofPoint oder andere SendMail-Messagingsysteme weiterleiten und Verzögerungen beim Senden von E-Mails an Exchange Online auftreten, finden Sie weitere Informationen unter [Konfigurieren von Proofpoint Email Protection mit Exchange Online](https://docs.microsoft.com/exchange/troubleshoot/email-delivery/configure-proofpoint-with-exchange).
- Wenn das Problem in Outlook Web App nicht auftritt, handelt es sich wahrscheinlich um ein Clientproblem. Versuchen Sie, das Profil neu zu erstellen.  
- Um nach verzögerten E-Mail-Problemen zu suchen, können Sie [die Nachrichtenablaufverfolgung](https://admin.exchange.microsoft.com/#/messagetrace) ausführen.  
- Führen Sie für Verzögerungen bei eingehenden E-Mails einen [Test für eingehende SMTP-E-Mails aus](https://testconnectivity.microsoft.com/tests/O365InboundSmtp/input). Führen Sie für Probleme im Zusammenhang mit ausgehenden E-Mails [den Test für ausgehende SMTP-E-Mails](https://testconnectivity.microsoft.com/tests/O365OutboundSmtp/input) aus.
