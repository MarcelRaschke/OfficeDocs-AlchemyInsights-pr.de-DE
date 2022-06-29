---
title: Synchronisierten Benutzer verwalten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 43918c35edbca92b4c2ceb19701f9c019c6ef5a7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66365961"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Die primäre E-Mail-Adresse kann nicht festgelegt, Benutzerattribute geändert oder ein synchronisierter Benutzer entfernt/gelöscht werden.

Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer- oder Objektattribute nicht mithilfe der Microsoft 365 Admin Center geändert werden.

Um synchronisierte Benutzer und alle ihre Attribute vollständig zu verwalten, verwenden Sie Ihre lokalen Active Directory-Benutzer und gruppenverwaltungskonsole (adsiedit.msc).  

Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in den folgenden gängigen Beispielen gezeigt:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
