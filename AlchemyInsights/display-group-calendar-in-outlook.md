---
title: 'Schritte zum Sichtbarmachen Microsoft 365 Gruppenkalenders in Outlook und OWA '
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800008"
- "16401"
ms.date: 01/21/2022
ms.openlocfilehash: 5c71f0b16b684040e5b58b19267b29eee39ebc0c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62760203"
---
# <a name="steps-to-make-microsoft-365-group-calendar-visible-in-outlook-and-owa"></a>Schritte zum Sichtbarmachen Microsoft 365 Gruppenkalenders in Outlook und OWA

Verwenden Sie die folgenden EXO PowerShell-Befehle, um einen Gruppenkalender (im Zusammenhang mit Microsoft Teams) in Outlook und OWA anzuzeigen:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$false`

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$false`

Detaillierte Anweisungen finden Sie unter [Ausblenden von Office 365-Gruppen auf der GAL und Exchange-Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
