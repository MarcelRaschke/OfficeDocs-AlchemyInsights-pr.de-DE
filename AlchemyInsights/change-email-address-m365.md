---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 3d5cea5a063329ac9ba91d95d458df8126143ff9
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61959007"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams

Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams über das [Microsoft 365 Admin Center](https://admin.microsoft.com/) ändern. Wählen Sie einfach die betreffende Gruppe und dann @bearbeiten E-Mail-Adresse aus.

Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe bzw. von Teams zu ändern:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Beispiel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
