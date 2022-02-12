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
ms.openlocfilehash: adb123b77d11c7dc9673eb12b8c8f8d447f5539b
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62614632"
---
# <a name="unable-to-change-username"></a>Benutzername (UserName) kann nicht geändert werden

In einigen Fällen werden UPN-Änderungen (UserPrincipalName) nicht in die Cloud übertragen. Möglicherweise erhalten Sie Validierungsfehler im Office 365-Portal oder können den Benutzernamen oder die E-Mail-Adresse nicht ändern. Um dieses Problem zu beheben, legen Sie "UserPrincipalName" mit diesem PowerShell-Befehl manuell fest.

**Beispiel: Umbenennen eines Benutzers**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Mit diesem Befehl wird "davidc@contoso.com" in "davidchew@contoso.com" umbenannt.

Weitere Informationen finden Sie unter [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0&preserve-view=true).
