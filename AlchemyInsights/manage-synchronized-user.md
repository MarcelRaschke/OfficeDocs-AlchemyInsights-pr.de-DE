---
title: Verwalten des synchronisierten Benutzers
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
- "9000609"
- "2444"
ms.openlocfilehash: 6f09bac7b7d4ea092ad89ed2d371a69eb8421379
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62575155"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Primäre E-Mail-Adresse kann nicht festgelegt, Benutzerattribute geändert oder synchronisierte Benutzer entfernt/gelöscht werden

Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer- oder Objektattribute nicht mithilfe der Microsoft 365 Admin Center geändert werden.

Um synchronisierte Benutzer und alle ihre Attribute vollständig zu verwalten, verwenden Sie Die lokale Active Directory-Verwaltungskonsole (adsiedit.msc).  

Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in diesen allgemeinen Beispielen gezeigt:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
