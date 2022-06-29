---
title: Benutzername (UserName) kann nicht geändert werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000183"
- "1729"
ms.date: 07/24/2020
ms.openlocfilehash: 4d3635d7b9b2eec51e7a31268cb1be699ea5f535
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66344901"
---
# <a name="unable-to-change-username"></a>Benutzername (UserName) kann nicht geändert werden

In einigen Fällen werden UPN-Änderungen (UserPrincipalName) nicht in die Cloud übertragen. Möglicherweise erhalten Sie Validierungsfehler im Office 365-Portal oder können den Benutzernamen oder die E-Mail-Adresse nicht ändern. Um dieses Problem zu beheben, legen Sie "UserPrincipalName" mit diesem PowerShell-Befehl manuell fest.

**Beispiel: Umbenennen eines Benutzers**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Mit diesem Befehl wird "davidc@contoso.com" in "davidchew@contoso.com" umbenannt.

Weitere Informationen finden Sie unter [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0&preserve-view=true).
