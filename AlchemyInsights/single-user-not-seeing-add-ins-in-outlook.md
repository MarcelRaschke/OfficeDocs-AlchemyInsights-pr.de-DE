---
title: Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 5a4fe5d23cf840fb3cb940bc78199ea94da40647
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65729836"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt

Der Benutzer ist möglicherweise Teil einer Rolle, die nicht über den richtigen AppsForOfficeEnabled-Parameter verfügt. Führen Sie dieses Cmdlet aus, um zu ermitteln, ob dem Benutzer die richtige Rolle zugeordnet ist:

`Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType`

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
