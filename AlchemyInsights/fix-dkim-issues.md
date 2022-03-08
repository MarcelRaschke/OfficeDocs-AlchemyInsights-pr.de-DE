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
ms.localizationpriority: medium
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: ae4032b2f54664ab6351b56fe8b37c0bf6e09b76
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63172543"
---
# <a name="fix-dkim-setup-issues"></a>Beheben von DKIM-Setupproblemen

Wenn Beim Aktivieren von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:

- Die meisten DKIM-Setupprobleme beziehen sich auf falsche DNS-Einträge. Stellen Sie sicher, dass der DKIM-CNAME-Eintrag (**kein** TXT-Eintrag) korrekt formatiert ist. Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge verteilt werden.

- Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, können Sie ihre benutzerdefinierte Domäne (z. B. contoso.com) ersetzen \<CustomDomain\> und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) ausführen: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
