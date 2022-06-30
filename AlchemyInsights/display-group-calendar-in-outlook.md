---
title: 'Schritte zum Anzeigen des Microsoft 365-Gruppenkalenders in Outlook und OWA '
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3800008"
- "16401"
ms.date: 01/21/2022
ms.openlocfilehash: dda2e1d3f5f2ff8fe0cadb184aa204121af69da7
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66511350"
---
# <a name="steps-to-make-microsoft-365-group-calendar-visible-in-outlook-and-owa"></a>Schritte zum Anzeigen des Microsoft 365-Gruppenkalenders in Outlook und OWA

Verwenden Sie die folgenden EXO PowerShell-Befehle, um einen Gruppenkalender (im Zusammenhang mit Microsoft Teams) in Outlook und OWA anzuzeigen:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$false`

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$false`

Detaillierte Anweisungen finden Sie unter [Ausblenden von Office 365-Gruppen auf der GAL und Exchange-Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
