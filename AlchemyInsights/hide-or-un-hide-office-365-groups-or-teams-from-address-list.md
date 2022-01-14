---
title: Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden
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
- "9002947"
- "5642"
ms.openlocfilehash: 28b2533c19e92dffb22532d84c9e42e5c3fac6c9
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61986781"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden

Verwenden Sie den folgenden EXO PowerShell-Befehl, um Office 365-Gruppen/-Teams auf Adresslisten (Globale Adressliste, GAL) von Exchange-Clients (Outlook, OWA) aus- oder einzublenden:

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Verwenden Sie den folgenden EXO PowerShell-Befehl, um die Office 365-Gruppen/-Teams von Exchange-Clients (Outlook, OWA) aus oder einzublenden:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detaillierte Anweisungen finden Sie unter [Ausblenden von Office 365-Gruppen auf der GAL und Exchange-Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
