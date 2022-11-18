---
title: Massenhinzufügen von Mitgliedern zu einer Microsoft 365-Gruppe
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200017"
- "16572"
ms.date: 01/28/2022
ms.openlocfilehash: 8e389c9b907ac129c4f00cd6ebb0d8c6375e6672
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66343713"
---
# <a name="bulk-add-members-to-a-microsoft-365-group"></a>Massenhinzufügen von Mitgliedern zu einer Microsoft 365-Gruppe

Hier ist ein EXO PowerShell-Befehl zum Massenhinzufügen von Benutzern zu einer Microsoft 365-Gruppe:

```PowerShell
$users= Get-User -ResultSize unlimited | ?{$_.Department -eq "Marketing" -AND $_.RecipientType -eq "UserMailbox"}
Add-UnifiedGroupLinks -Identity Marketing -LinkType members -Links ($users.UserPrincipalName)
```

Schritte zum Hinzufügen von Mitgliedern zu einer Gruppe mithilfe einer CSV-Datei finden Sie [unter Massenhinzufügen von Gruppenmitgliedern in Azure Active Directory](https://aka.ms/M365GroupMemberBulkAddCSV).
