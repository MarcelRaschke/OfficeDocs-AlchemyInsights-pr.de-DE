---
title: Verwalten des synchronisierten Benutzers
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114777"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Primäre E-Mail-Adresse kann nicht festgelegt, Benutzerattribute geändert oder synchronisierte Benutzer entfernt/gelöscht werden

Wenn die Verzeichnissynchronisierung für Ihre Umgebung aktiviert ist, können einige Benutzer- oder Objektattribute nicht mithilfe der Microsoft 365 Admin Center geändert werden.

Um synchronisierte Benutzer und alle ihre Attribute vollständig zu verwalten, verwenden Sie Die lokale Active Directory-Verwaltungskonsole (adsiedit.msc).  

Alternativ können Sie einzelne Benutzer oder Attribute für synchronisierte Benutzer mithilfe von PowerShell ändern, wie in diesen allgemeinen Beispielen gezeigt:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
