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
ms.openlocfilehash: ac4d19d39799a040618674c7bfde3998f621acc1
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62669227"
---
# <a name="how-to-enable-hosted-voicemail"></a>So aktivieren Sie gehostete Voicemail

Um Voicemail zu aktivieren, muss **HostedVoicemail** auf $true festgelegt werden.

Die **HostedVoicemail-Eigenschaft** für den Benutzer mithilfe von Remote PowerShell (RPS).

Weitere Informationen zum Herstellen einer Verbindung mit RPS finden Sie [in Microsoft Teams PowerShell-Übersicht](https://docs.microsoft.com/microsoftteams/teams-powershell-overview), um weitere Informationen zum Herstellen einer Verbindung mit RPS zu finden.

1. Der Teams-Administrator sollte für Teams bei Remote-PowerShell angemeldet sein.
1. Über PowerShell-Aufforderung kann der Teams Administrator **set-csuser user@contoso.com -HostedVoiceMail $true** ausführen, wobei der SIP-URI des betreffenden Benutzers ist.

**Hinweis**: Es kann bis zu 24 Stunden dauern, bis Änderungen an Richtlinien repliziert wurden.