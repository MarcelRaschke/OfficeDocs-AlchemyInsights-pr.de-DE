---
title: Kalenderberechtigungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 647800ac897a96552105a754f95b00a550bc20a5
ms.sourcegitcommit: 8324c868c664bfdee6d5bb99ad8d41e9dd46d10f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66540170"
---
# <a name="calendar-permissions"></a>Kalenderberechtigungen

Benutzer können ihre eigenen Kalenderberechtigungen mit Outlook im Web oder anderen Clients ändern, aber als Administrator müssen Sie dies möglicherweise ebenfalls untersuchen.  
Mit dem Exchange PowerShell-Cmdlet können Sie die Berechtigung für den Kalender eines Benutzers anzeigen:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Weitere Informationen finden Sie in den folgenden Themen:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps&preserve-view=true)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps&preserve-view=true)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenderberechtigungen werden bei der Freigabe von Kalendern verwendet. Weitere Informationen zum Freigeben eines Outlook-Kalenders finden Sie in den folgenden Artikeln:

- [Freigeben eines Outlook-Kalenders für andere Personen](https://support.microsoft.com/office/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Freigeben Ihres Kalenders in Outlook im Web for Business](https://support.microsoft.com/office/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Um Probleme mit Kalenderberechtigungen zu beheben, können Sie das [Tool "Support- und Wiederherstellungs-Assistent"](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) verwenden.