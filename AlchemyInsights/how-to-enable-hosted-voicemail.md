---
title: So aktivieren Sie gehostete Voicemail
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318647"
---
# <a name="how-to-enable-hosted-voicemail"></a>So aktivieren Sie gehostete Voicemail

Um Voicemail zu aktivieren, muss **HostedVoicemail** auf $true festgelegt werden.

Die **HostedVoicemail-Eigenschaft** für den Benutzer mithilfe von Remote PowerShell (RPS).

Weitere Informationen zum Herstellen einer Verbindung mit RPS finden Sie [in Microsoft Teams PowerShell-Übersicht,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) um weitere Informationen zum Herstellen einer Verbindung mit RPS zu finden.

1. Der Teams-Administrator sollte für Teams bei Remote-PowerShell angemeldet sein.
1. Über powerShell-Aufforderung kann der Teams Administrator **set-csuser user@contoso.com -HostedVoiceMail $true** ausführen, wobei der SIP-URI des betreffenden Benutzers ist.

**Hinweis:** Es kann bis zu 24 Stunden dauern, bis Änderungen an Richtlinien repliziert wurden.