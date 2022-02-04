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
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: c594c17120793ab2c2de6518a23a4d78f2c76a59
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61936229"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt

Der Benutzer gehört möglicherweise zu einer Rolle, die nicht über den richtigen AppsForOfficeEnabled-Parameter verfügt. Führen Sie dieses Cmdlet aus, um zu ermitteln, ob dem Benutzer die richtige Rolle zugeordnet ist:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
