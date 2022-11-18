---
title: So aktivieren Sie gehostete Voicemail
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002347"
- "7563"
ms.date: 12/09/2020
ms.openlocfilehash: b1b0dbf1aceaf4fe2774bd85d53fb97cd0cf9b96
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66388965"
---
# <a name="how-to-enable-hosted-voicemail"></a>So aktivieren Sie gehostete Voicemail

Um Voicemail zu aktivieren, muss **HostedVoicemail** auf $true festgelegt sein.

Die **HostedVoicemail-Eigenschaft** für den Benutzer, der Remote PowerShell (RPS) verwendet.

Weitere Informationen zum Herstellen einer Verbindung mit RPS finden Sie unter [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.

1. Die Teams-Admin sollten bei Remote PowerShell für Teams angemeldet sein.
1. Über die PowerShell-Eingabeaufforderung kann der **Teams-Admin set-csuser user@contoso.com -HostedVoiceMail $true** ausführen, in dem sich der SIP-URI des betreffenden Benutzers befindet.

**Hinweis**: Das Replizieren von Änderungen an Richtlinien kann bis zu 24 Stunden dauern.