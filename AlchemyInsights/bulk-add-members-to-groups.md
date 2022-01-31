---
title: Massenzufügen von Mitgliedern zu einer Microsoft 365 Gruppe
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
- "1200017"
- "16572"
ms.date: 01/28/2022
ms.openlocfilehash: 1cc746c0a68d649d40102c25bde3eeea3fb27c17
ms.sourcegitcommit: 0bf8e159e9e49792db04709867d4f78e1047aa73
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/31/2022
ms.locfileid: "62281106"
---
# <a name="bulk-add-members-to-a-microsoft-365-group"></a>Massenzufügen von Mitgliedern zu einer Microsoft 365 Gruppe

Nachfolgend sehen Sie einen EXO PowerShell-Befehl, mit dem Benutzer einer Microsoft 365 Gruppe in massenweiser Reihenfolge hinzugefügt werden können:

```PowerShell
$users= Get-User -ResultSize unlimited | ?{$_.Department -eq "Marketing" -AND $_.RecipientType -eq "UserMailbox"}
Add-UnifiedGroupLinks -Identity Marketing -LinkType members -Links ($users.UserPrincipalName)
```

Schritte zum Hinzufügen von Mitgliedern zu einer Gruppe mithilfe einer CSV-Datei finden Sie unter [Massenhinzufügen von Gruppenmitgliedern in Azure Active Directory](https://aka.ms/M365GroupMemberBulkAddCSV).
