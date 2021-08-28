---
title: Beheben von DKIM-Setupproblemen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945930"
---
# <a name="fix-dkim-setup-issues"></a>Beheben von DKIM-Setupproblemen

Wenn Beim Aktivieren von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:

- Die meisten DKIM-Setupprobleme beziehen sich auf falsche DNS-Einträge. Überprüfen Sie, ob der DKIM CNAME-Eintrag **(kein** TXT-Eintrag) richtig formatiert ist. Weitere Informationen finden Sie in diesem [Thema.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge verteilt werden.

- Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, können Sie \<CustomDomain\> durch Ihre benutzerdefinierte Domäne (z. B. contoso.com) ersetzen und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ausführen: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
