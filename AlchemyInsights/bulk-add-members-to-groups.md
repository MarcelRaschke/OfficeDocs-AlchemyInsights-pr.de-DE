---
title: Massenzufügen von Mitgliedern zu einer Microsoft 365 Gruppe
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1200017"
- "16572"
ms.date: 01/28/2022
ms.openlocfilehash: 1aca1d84a443c6a481d15c65977c4665a8949873
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63163687"
---
# <a name="bulk-add-members-to-a-microsoft-365-group"></a>Massenzufügen von Mitgliedern zu einer Microsoft 365 Gruppe

Nachfolgend sehen Sie einen EXO PowerShell-Befehl, mit dem Benutzer einer Microsoft 365 Gruppe massenweise hinzugefügt werden können:

```PowerShell
$users= Get-User -ResultSize unlimited | ?{$_.Department -eq "Marketing" -AND $_.RecipientType -eq "UserMailbox"}
Add-UnifiedGroupLinks -Identity Marketing -LinkType members -Links ($users.UserPrincipalName)
```

Schritte zum Hinzufügen von Mitgliedern zu einer Gruppe mithilfe einer CSV-Datei finden Sie unter [Massenhinzufügen von Gruppenmitgliedern in Azure Active Directory](https://aka.ms/M365GroupMemberBulkAddCSV).
