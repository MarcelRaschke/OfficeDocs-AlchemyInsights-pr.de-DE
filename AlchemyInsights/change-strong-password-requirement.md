---
title: Ändern der Anforderung für sichere Kennwörter
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 4fedfa927b03051f3dad1992677c5bf74e2ff1d1
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62579565"
---
# <a name="change-strong-password-requirement"></a>Ändern der Anforderung eines sicheren Kennworts

Microsoft erfordert standardmäßig sichere Kennwörter.

Mithilfe von PowerShell können Sie sichere Kennwörter für bestimmte Benutzer mit den folgenden Befehlen deaktivieren:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Um sichere Kennwörter für alle Benutzer zu deaktivieren, verwenden Sie Folgendes:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Weitere Informationen zur Kennwortrichtlinie](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Herstellen einer Verbindung mit Microsoft 365 mit PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Weitere Informationen zu PowerShell-MsolUser-Befehlen](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0&preserve-view=true)
