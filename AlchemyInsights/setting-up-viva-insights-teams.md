---
title: Einrichten der Viva Insights-App in Teams
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010268"
- "16697"
ms.date: 02/15/2022
ms.openlocfilehash: baaa1c7459eb4b5d014c3cc515d0b45f14b7fc86
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66316047"
---
# <a name="setting-up-the-viva-insights-app-in-teams"></a>Einrichten der Viva Insights-App in Teams

Informationen zum Einrichten und Konfigurieren Viva Insights App in Teams finden Sie unter:

- [Admin von Aufgaben für Viva Insights](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app-admin-tasks)
- [Installieren und Anheften der Viva Insights-App](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app-install#install-the-app)

**Hinweis** Um die Viva Insights-App zu finden, wechseln Sie zu [`https://aka.ms/InsightsTeamsApp`](https://aka.ms/InsightsTeamsApp).

Stellen Sie außerdem sicher, [dass Sie EWSAllowList](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#q7-why-cant-licensed-users-see-one-or-more-of-the-viva-insights-or-myanalytics-elements) konfigurieren. Beispiel:

Verwenden Sie `Set-CASMailbox` das Cmdlet, um *WeveEngine/** und *MyAnalytics/** zu *EwsAllowList* für betroffene Benutzer hinzuzufügen:

`Set-CASMailbox [USER ID] -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Oder Sie können diese Änderung auf Mandantenebene vornehmen, indem Sie für jede die folgenden PowerShell-Cmd ausführen:

`Set-OrganizationConfig -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Weitere Informationen finden Sie unter:

- [Häufig gestellte Fragen zu persönlichen Insights für Administratoren](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#for-it-administrators)
- [Viva Insights in Teams](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app)
- [Häufig gestellte Fragen zu persönlichen Einblicken in Teams](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app-faq)
