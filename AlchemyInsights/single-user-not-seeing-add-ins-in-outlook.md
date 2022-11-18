---
title: Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom: ''
ms.date: 07/16/2020
ms.openlocfilehash: 3543ddcaa7947e515bc02e5bc2c8df23464958db
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66425578"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Einem einzelnen Benutzer werden keine Add-Ins in Outlook angezeigt

Der Benutzer ist möglicherweise Teil einer Rolle, die nicht über den richtigen AppsForOfficeEnabled-Parameter verfügt. Führen Sie dieses Cmdlet aus, um zu ermitteln, ob dem Benutzer die richtige Rolle zugeordnet ist:

`Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType`

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
