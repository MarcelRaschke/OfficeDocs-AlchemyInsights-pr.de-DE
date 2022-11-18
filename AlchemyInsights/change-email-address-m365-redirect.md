---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: dded049d385f229e70b22c9805ba6c2c198d8c61
ms.sourcegitcommit: 427a2af98183d8255b059b72b58c5c5e75e02d5e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/13/2022
ms.locfileid: "67652165"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams

Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams über das [Microsoft 365 Admin Center](https://admin.microsoft.com/adminportal/home?ref=homepage) ändern. Wählen Sie einfach die betreffende Gruppe und dann „E-Mail-Adresse @bearbeiten“ aus.

Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe bzw. von Teams zu ändern:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Beispiel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
