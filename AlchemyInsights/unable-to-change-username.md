---
title: Benutzername (UserName) kann nicht geändert werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: ee0d4c22c1f58eab7b3f01377bfbd4ab3a143a90
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61988329"
---
# <a name="unable-to-change-username"></a>Benutzername (UserName) kann nicht geändert werden

In einigen Fällen werden UPN-Änderungen (UserPrincipalName) nicht in die Cloud übertragen. Möglicherweise erhalten Sie Validierungsfehler im Office 365-Portal oder können den Benutzernamen oder die E-Mail-Adresse nicht ändern. Um dieses Problem zu beheben, legen Sie "UserPrincipalName" mit diesem PowerShell-Befehl manuell fest.

**Beispiel: Umbenennen eines Benutzers**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Mit diesem Befehl wird "davidc@contoso.com" in "davidchew@contoso.com" umbenannt.

Weitere Informationen finden Sie unter [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0&preserve-view=true).
