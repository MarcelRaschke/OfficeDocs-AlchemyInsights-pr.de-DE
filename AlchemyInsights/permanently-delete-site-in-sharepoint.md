---
title: Endgültiges Löschen einer Site in SharePoint
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "5200006"
- "4391"
ms.openlocfilehash: 5468eaa64a0b1f8493299faff2e78972af20543e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66305535"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Endgültiges Löschen einer Site in SharePoint

Um eine URL von einer gelöschten Site wiederzuverwenden (zum Neuerstellen einer Site) oder um eine Site endgültig zu löschen, weil sie nicht mehr verwendet wird, können Sie **Endgültig löschen** im neuen SharePoint Admin Center verwenden. 

1. Wechseln Sie zur [Seite „Gelöschte Sites“ im neuen SharePoint Admin Center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true), und melden Sie sich mit einem Konto an, das über Administratorberechtigungen für Ihre Organisation verfügt. 

2. Wählen Sie in der linken Spalte eine Site aus. 

3. Klicken Sie auf **Endgültig löschen**. 

**Hinweis**: Mit Gruppen verbundene Sites können über das neue SharePoint Admin Center nicht endgültig gelöscht werden. Stattdessen müssen Sie [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) verwenden.  

Weitere Informationen finden Sie unter [Endgültiges Löschen einer Site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
