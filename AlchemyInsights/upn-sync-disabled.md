---
title: UPN-Synchronisierung deaktiviert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038111"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie vor dem 30. März 2016 mit der Synchronisierung mit Azure AD begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um nur die upn soft match für Ihre Organisation zu aktivieren:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Upn soft match is automatically turned for organizations that started syncing to Azure AD on or after March 30, 2016.
  
Weitere Informationen zum Aktivieren der Soft-Match für UPN und andere Synchronisierungsfeatures finden Sie unter [Azure AD Verbinden Synchronisierungsdienstfeatures.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

