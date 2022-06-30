---
title: Ihr Archivpostfach ist fast voll
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100006"
- "7960"
ms.date: 01/25/2021
ms.openlocfilehash: dfa339329119203e3ef7df794dbea9033845d19d
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66528529"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Ihr Archivpostfach ist fast voll

Wenn der Benutzer die Warnung erhält; **Ihr Archivpostfach ist fast voll**, oder Sie müssen die Größe des Archivpostfachs erhöhen. Hier sind einige Tipps:

1. Wenn dem Benutzer eine Exchange Online Plan 1 zugewiesen ist, führen Sie ein Upgrade auf **Exchange Online Plan 2-Lizenz** durch, um die Größe von 50 GB auf 100 GB zu erhöhen.
1. Wenn dem Benutzer bereits eine der folgenden Optionen zugewiesen ist: **Exchange Online Plan 2** oder einen Exchange Online Plan 1 mit einem Exchange Online-Archivierung-Add-On, führen Sie die folgenden Schritte aus, um die automatisch erweiterte Archivierung zu aktivieren:.

    1. [Stellen Sie eine Verbindung mit Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) her.
    2. Führen Sie das folgende Befehlslet für den Benutzer aus:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    3. Führen Sie das folgende Befehlslet aus, um zu bestätigen, dass es für den Benutzer aktiviert ist:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Weitere Informationen finden Sie unter:

- [Unbegrenzte Archivierung aktivieren – Admin Hilfe – Microsoft 365 Compliance | Microsoft-Dokumentation](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online-Grenzwerte – Dienstbeschreibungen | Microsoft-Dokumentation](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Upgrade auf einen anderen Geschäftsplan | Microsoft-Dokumentation](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)
