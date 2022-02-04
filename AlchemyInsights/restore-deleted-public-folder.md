---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
  - 3500007
  - 3488
---

# <a name="restore-a-deleted-public-folder"></a>Wiederherstellen eines gelöschten öffentlichen Ordners

**So stellen Sie gelöschte Elemente aus einem öffentlichen Ordner wieder her:**

- Siehe ["Gelöschte Elemente können nicht aus einem öffentlichen Ordner ohne E-Mail-Nachrichten in Outlook 2016 wiederhergestellt](https://aka.ms/pfrec)werden."
 
**So stellen Sie einen gelöschten öffentlichen Ordner (eines beliebigen Typs) wieder her:** 

- Verwenden Sie den folgenden EXO PowerShell-Befehl:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Beispiel: Mit dem folgenden Befehl wird "Subfolder1" wiederhergestellt und unter "\Parent1" platziert:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Weitere Informationen finden Sie unter [Wiederherstellen eines gelöschten öffentlichen Ordners.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
