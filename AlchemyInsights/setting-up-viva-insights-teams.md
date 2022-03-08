---
title: Einrichten der Viva Insights-App in Teams
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9010268"
- "16697"
ms.date: 02/15/2022
ms.openlocfilehash: d63264fc7f03624932a93d5d348391f5a87b5398
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63157963"
---
# <a name="setting-up-the-viva-insights-app-in-teams"></a>Einrichten der Viva Insights-App in Teams

Informationen zum Einrichten und Konfigurieren der Viva Insights-App in Teams finden Sie unter:

- [Administratoraufgaben für Viva Insights](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app-admin-tasks)
- [Installieren und Anheften der Viva Insights-App](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app-install#install-the-app)

**Hinweis** Um die Viva Insights-App zu finden, wechseln Sie zu [`https://aka.ms/InsightsTeamsApp`](https://aka.ms/InsightsTeamsApp).

Stellen Sie außerdem sicher, dass [Sie EWSAllowList](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#q7-why-cant-licensed-users-see-one-or-more-of-the-viva-insights-or-myanalytics-elements) konfigurieren. Beispiel:

Verwenden Sie `Set-CASMailbox` das Cmdlet, um *WeveEngine/** und *MyAnalytics/** zu *EwsAllowList* für betroffene Benutzer hinzuzufügen:

`Set-CASMailbox [USER ID] -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Sie können diese Änderung auch auf Mandantenebene vornehmen, indem Sie die folgende PowerShell-Cmd für jeden ausführen:

`Set-OrganizationConfig -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Weitere Informationen finden Sie unter:

- [Häufig gestellte Fragen zu persönlichen Insights für Administratoren](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#for-it-administrators)
- [Viva Insights in Teams](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app)
- [Persönliche Einblicke in häufig gestellte Fragen Teams](https://docs.microsoft.com/viva/insights/personal/teams/viva-teams-app-faq)
