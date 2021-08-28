---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819079"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams

Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams über das [Microsoft 365 Admin Center](https://admin.microsoft.com/) ändern. Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.

Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe bzw. von Teams zu ändern:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Beispiel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
