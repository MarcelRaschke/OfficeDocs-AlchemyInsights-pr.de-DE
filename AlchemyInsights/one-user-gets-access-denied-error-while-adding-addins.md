---
title: Ein Benutzer erhält beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "6700008"
- "5892"
ms.date: 07/23/2020
ms.openlocfilehash: c4765fbf581645660b15439f1cbc8bfd258b72bf
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66336405"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Ein Benutzer erhält beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“

Benutzer-PowerShell, um Berechtigungen zu finden:

Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType