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
ms.openlocfilehash: 9338a7ea813eb823aff5757ec7379af5b68c9e2d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63211401"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt

Der Benutzer gehört möglicherweise zu einer Rolle, die nicht über den richtigen AppsForOfficeEnabled-Parameter verfügt. Führen Sie dieses Cmdlet aus, um zu ermitteln, ob dem Benutzer die richtige Rolle zugeordnet ist:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
