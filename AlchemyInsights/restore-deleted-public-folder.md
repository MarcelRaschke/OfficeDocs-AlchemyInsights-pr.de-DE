---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
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
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943374"
---
# <a name="restore-a-deleted-public-folder"></a>Wiederherstellen eines gelöschten öffentlichen Ordners

**So stellen Sie gelöschte Elemente aus einem öffentlichen Ordner wieder her:**

- See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).
 
**So stellen Sie einen gelöschten öffentlichen Ordner (eines beliebigen Typs) wieder her:** 

- Verwenden Sie den folgenden EXO PowerShell-Befehl:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Beispiel: Mit dem folgenden Befehl wird Subfolder1 wiederhergestellt und unter "\Parent1" platziert:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Weitere Informationen finden Sie unter [Wiederherstellen eines gelöschten öffentlichen Ordners.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
