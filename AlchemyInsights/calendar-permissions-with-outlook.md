---
title: Kalenderberechtigungen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046103"
---
# <a name="calendar-permissions"></a>Kalenderberechtigungen

Benutzer können ihre eigenen Kalenderberechtigungen mit Outlook im Web oder anderen Clients ändern, aber als Administrator müssen Sie möglicherweise auch untersuchen.  
Mit Exchange PowerShell-Cmdlet wird Ihnen die Berechtigung im Kalender eines Benutzers angezeigt:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Weitere Informationen finden Sie unter:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenderberechtigungen werden bei der Freigabe von Kalendern verwendet. Weitere Informationen zum Freigeben eines Outlook Kalenders finden Sie in den folgenden Artikeln:

- [Freigeben eines Outlook-Kalenders für andere Personen](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Freigeben Ihres Kalenders in Outlook im Web for Business](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Zur Problembehandlung von Kalenderberechtigungen können Sie das [tool Support- und Wiederherstellungs-Assistent](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) verwenden.