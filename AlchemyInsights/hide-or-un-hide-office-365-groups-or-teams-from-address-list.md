---
title: Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 9656d97901468d886120e76f8b685dc134ae3ac9
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66268516"
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
