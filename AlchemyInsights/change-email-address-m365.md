---
title: Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a907c92a37d714bc7101365220401c552eb3aeed
ms.sourcegitcommit: 5afc3c4a1270409ed3691c90ba139878d845e7a3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "66010670"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Ändern der E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams

Sie können die E-Mail-Adresse einer Microsoft 365-Gruppe oder von Microsoft Teams über das [Microsoft 365 Admin Center](https://admin.microsoft.com/adminportal/home?ref=homepage) ändern. Wählen Sie einfach die betreffende Gruppe und dann „E-Mail-Adresse @bearbeiten“ aus.

Sie können auch den folgenden EXO PowerShell-Befehl verwenden, um die primäre SMTP-Adresse einer Microsoft 365-Gruppe bzw. von Teams zu ändern:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Beispiel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
