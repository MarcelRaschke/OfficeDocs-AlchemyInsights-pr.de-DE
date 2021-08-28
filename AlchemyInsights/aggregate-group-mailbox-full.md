---
title: AggregateGroupMailbox vollständiger NDR, der für E-Mails empfangen wurde, die an Microsoft 365 Gruppe gesendet wurden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315909"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox vollständiger NDR, der für E-Mails empfangen wurde, die an Microsoft 365 Gruppe gesendet wurden

Verwenden Sie den folgenden EXO Shell-Befehl, um eine Exchange Transportregel zum automatischen Ablegen von E-Mails zu erstellen, die an das aggregierte Gruppenpostfach gesendet werden:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Hinweis:** Ersetzen Sie die SMTP-Adresse in **"-SentTo"** durch die SMTP-Adresse des aggregierten Gruppenpostfachs in Ihrem Mandanten. Sie können die SMTP-Adresse des Aggregatgruppenpostfachs vom empfangenen NDR abrufen.



