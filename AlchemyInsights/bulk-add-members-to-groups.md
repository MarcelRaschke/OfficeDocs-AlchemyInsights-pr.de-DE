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
ms.openlocfilehash: bc2ea0c3aa0b01a1b6fdd745656b0477561d447d
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62626081"
---
# <a name="bulk-add-members-to-a-microsoft-365-group"></a>Massenzufügen von Mitgliedern zu einer Microsoft 365 Gruppe

Nachfolgend sehen Sie einen EXO PowerShell-Befehl, mit dem Benutzer einer Microsoft 365 Gruppe in massenweiser Reihenfolge hinzugefügt werden können:

```PowerShell
$users= Get-User -ResultSize unlimited | ?{$_.Department -eq "Marketing" -AND $_.RecipientType -eq "UserMailbox"}
Add-UnifiedGroupLinks -Identity Marketing -LinkType members -Links ($users.UserPrincipalName)
```

Schritte zum Hinzufügen von Mitgliedern zu einer Gruppe mithilfe einer CSV-Datei finden Sie unter [Massenhinzufügen von Gruppenmitgliedern in Azure Active Directory](https://aka.ms/M365GroupMemberBulkAddCSV).
