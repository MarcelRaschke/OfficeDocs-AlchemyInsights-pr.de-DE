---
title: UPN-Synchronisierung deaktiviert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 568cd6683c78d7e5961fbded043e7786f32530f1
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63209372"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie die Synchronisierung mit Azure AD vor dem 30. März 2016 begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um nur die upn soft match für Ihre Organisation zu aktivieren:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Upn soft match is automatically turned for organizations that started syncing to Azure AD on or after March 30, 2016.
  
Weitere Informationen zum Aktivieren der Soft-Match für UPN und andere Synchronisierungsfunktionen finden Sie unter [Azure AD Verbinden Features des Synchronisierungsdiensts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

