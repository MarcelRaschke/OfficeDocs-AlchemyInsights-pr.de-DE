---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: a803d35e94f2dfd18756b11a2c6817d7b5ae7da7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66264250"
---
# <a name="restore-a-deleted-public-folder"></a>Wiederherstellen eines gelöschten öffentlichen Ordners

**So stellen Sie gelöschte Elemente aus einem öffentlichen Ordner wieder her**:

- Siehe [Sie können gelöschte Elemente aus einem öffentlichen Ordner ohne E-Mail in Outlook 2016 nicht wiederherstellen](https://aka.ms/pfrec).
 
**So stellen Sie einen gelöschten öffentlichen Ordner (beliebigen Typs) wieder her**: 

- Verwenden Sie den folgenden EXO PowerShell-Befehl:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Beispiel: Mit dem folgenden Befehl wird der Unterordner1 wiederhergestellt und unter \Parent1 platziert:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Weitere Informationen finden [Sie unter Wiederherstellen eines gelöschten öffentlichen Ordners](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
