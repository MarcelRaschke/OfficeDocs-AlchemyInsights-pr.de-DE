---
title: Probleme mit Viva Insights Outlook-Add-In
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010264"
- "16696"
ms.date: 02/15/2022
ms.openlocfilehash: 40368fdcad57274d90bc938b2a89b2708ed6c020
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66338457"
---
# <a name="issues-with-viva-insights-outlook-add-in"></a>Probleme mit Viva Insights Outlook-Add-In

Informationen zum Aktivieren oder Deaktivieren des Viva Insights Outlook-Add-Ins finden Sie unter:  

- [Viva Insights Outlook-Add-In](https://docs.microsoft.com/viva/insights/personal/use/add-in)
- [Viva Insights Outlook-Add-In – Admin Aufgaben](https://docs.microsoft.com/viva/insights/personal/setup/configure#to-enable-access-to-viva-digest-emails-the-dashboard-and-the-viva-insights-outlook-add-in)

Stellen Sie außerdem sicher, [dass Sie EWSAllowList](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#q7-why-cant-licensed-users-see-one-or-more-of-the-viva-insights-or-myanalytics-elements) konfigurieren. Beispiel:

Verwenden Sie `Set-CASMailbox` das Cmdlet, um *WeveEngine/** und *MyAnalytics/** zu *EwsAllowList* für betroffene Benutzer hinzuzufügen:

`Set-CASMailbox [USER ID] -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Sie können diese Änderung auch auf Mandantenebene vornehmen, indem Sie jeweils die folgende PowerShell-Cmd ausführen:

`Set-OrganizationConfig -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Weitere Informationen finden Sie unter:

- [Viva Insights Bereitstellungshandbuch](https://docs.microsoft.com/viva/insights/personal/setup/deployment-guide)
- [Viva Insights von Plänen und Umgebungen](https://docs.microsoft.com/viva/insights/personal/overview/plans-environments)
- [Häufig gestellte Fragen zu persönlichen Insights für Administratoren](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#for-it-administrators)
