---
title: Ihr Archivpostfach ist fast voll
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 0a71ceedc20bbd1241d0ce4c582007c50eb4a7ba
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61957998"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Ihr Archivpostfach ist fast voll

Wenn der Benutzer die Warnung empfängt; **Ihr Archivpostfach ist fast voll,** oder Sie müssen die Größe des Archivpostfachs erhöhen. Hier sind einige Tipps:

1. Wenn dem Benutzer ein Exchange Online Plan 1 zugewiesen ist, führen Sie ein Upgrade auf **Exchange Online Plan 2-Lizenz** durch, um die Größe von 50 GB auf 100 GB zu erhöhen.
1. Wenn dem Benutzer bereits eine der folgenden Optionen zugewiesen ist: **Exchange Online Plan 2** oder ein Exchange Online Plan 1 mit einem Exchange Online-Archivierung-Add-On, führen Sie die folgenden Schritte aus, um die automatische Erweiterung der Archivierung zu aktivieren:

    1. [Verbinden zu Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Führen Sie das folgende Commandlet für den Benutzer aus:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    3. Führen Sie das folgende Commandlet aus, um zu bestätigen, dass es für den Benutzer aktiviert ist:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Weitere Informationen finden Sie unter:

- [Aktivieren der unbegrenzten Archivierung – Administratorhilfe – Microsoft 365 Compliance-| Microsoft-Dokumente](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [grenzwerte für Exchange Online – Dienstbeschreibungen | Microsoft-Dokumente](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade auf einen anderen Geschäftsplan | Microsoft-Dokumente](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)
