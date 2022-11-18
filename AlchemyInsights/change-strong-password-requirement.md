---
title: Starke Kennwortanforderung ändern
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 594f2fee8d369385f966fa8f5eef8e740e6783ff
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66395031"
---
# <a name="change-strong-password-requirement"></a>Ändern der Anforderung eines sicheren Kennworts

Microsoft erfordert standardmäßig sichere Kennwörter.

Mithilfe von PowerShell können Sie sichere Kennwörter für bestimmte Benutzer mit den folgenden Befehlen deaktivieren:

`Set-MsolUser -UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false`

Verwenden Sie Folgendes, um sichere Kennwörter für alle Benutzer zu deaktivieren:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Weitere Informationen zur Kennwortrichtlinie](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [So stellen Sie eine Verbindung mit Microsoft 365 mit PowerShell her](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Weitere Informationen zu PowerShell-MsolUser-Befehlen](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0&preserve-view=true)
