---
title: Ein Benutzer erhält beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
  - 5892
  - 6700008
---

# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Ein Benutzer erhält beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“

Benutzer-PowerShell, um Berechtigungen zu finden:

Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType