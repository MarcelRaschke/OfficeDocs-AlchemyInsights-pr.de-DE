---
title: Probleme mit Dem Viva Insights Outlook-Add-In
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
- "9010264"
- "16696"
ms.date: 02/15/2022
ms.openlocfilehash: 0eb1ced335a099b11db84e656737a895b8535c95
ms.sourcegitcommit: 5c192c14acfb55ca3d5bbee10bf0e5ccecef8bf2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/16/2022
ms.locfileid: "62860080"
---
# <a name="issues-with-viva-insights-outlook-add-in"></a>Probleme mit Dem Viva Insights Outlook-Add-In

Informationen zum Aktivieren oder Deaktivieren des Viva Insights Outlook-Add-Ins finden Sie unter:  

- [Viva Insights Outlook-Add-In](https://docs.microsoft.com/viva/insights/personal/use/add-in)
- [Viva Insights Outlook-Add-In – Administratoraufgaben](https://docs.microsoft.com/viva/insights/personal/setup/configure#to-enable-access-to-viva-digest-emails-the-dashboard-and-the-viva-insights-outlook-add-in)

Stellen Sie außerdem sicher, dass [Sie EWSAllowList](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#q7-why-cant-licensed-users-see-one-or-more-of-the-viva-insights-or-myanalytics-elements) konfigurieren. Zum Beispiel:

Verwenden Sie `Set-CASMailbox` das Cmdlet, um *WeveEngine/** und *MyAnalytics/** zu *EwsAllowList* für betroffene Benutzer hinzuzufügen:

`Set-CASMailbox [USER ID] -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Sie können diese Änderung auch auf Mandantenebene vornehmen, indem Sie jeweils die folgende PowerShell-Cmd ausführen:

`Set-OrganizationConfig -EwsApplicationAccessPolicy EnforceAllowList -EwsAllowList @{Add="WeveEngine/*","MyAnalytics/*"}`

Weitere Informationen finden Sie unter:

- [Bereitstellungshandbuch für Viva Insights](https://docs.microsoft.com/viva/insights/personal/setup/deployment-guide)
- [Viva Insights Pläne und Umgebungen](https://docs.microsoft.com/viva/insights/personal/overview/plans-environments)
- [Häufig gestellte Fragen zu persönlichen Insights für Administratoren](https://docs.microsoft.com/viva/insights/personal/overview/mya-faq#for-it-administrators)
