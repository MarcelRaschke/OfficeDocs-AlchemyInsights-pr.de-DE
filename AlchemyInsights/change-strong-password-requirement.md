---
title: Ändern der Anforderung für sichere Kennwörter
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
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070683"
---
# <a name="change-strong-password-requirement"></a>Ändern der Anforderung eines sicheren Kennworts

Microsoft erfordert standardmäßig sichere Kennwörter.

Mithilfe von PowerShell können Sie sichere Kennwörter für bestimmte Benutzer mit den folgenden Befehlen deaktivieren:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Um sichere Kennwörter für alle Benutzer zu deaktivieren, verwenden Sie Folgendes:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Weitere Informationen zur Kennwortrichtlinie](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Herstellen einer Verbindung mit Microsoft 365 mit PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Weitere Informationen zu PowerShell-MsolUser-Befehlen](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
