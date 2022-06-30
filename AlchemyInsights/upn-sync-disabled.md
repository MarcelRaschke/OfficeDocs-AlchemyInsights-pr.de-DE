---
title: UPN-Synchronisierung deaktiviert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.date: 04/21/2020
ms.openlocfilehash: 59c1994f213ef2ad5c218fc765559e55b27d844e
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66520253"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie vor dem 30. März 2016 mit der Synchronisierung mit Azure AD begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um nur upn soft match für Ihre Organisation zu aktivieren:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Die vorläufige UPN-Übereinstimmung wird automatisch für Organisationen aktiviert, die mit der Synchronisierung mit Azure AD am oder nach dem 30. März 2016 begonnen haben.
  
Weitere Informationen zum Aktivieren von soft match auf UPN und anderen Synchronisierungsfeatures finden Sie unter [den Features des Azure AD Connect-Synchronisierungsdiensts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

