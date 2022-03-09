---
title: Ein Benutzer erhält beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: e987b0b05062813cb9a2f81bfd71c02bc07332f5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63245933"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Ein Benutzer erhält beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“

Benutzer-PowerShell, um Berechtigungen zu finden:

Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType