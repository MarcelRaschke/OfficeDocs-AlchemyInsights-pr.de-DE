---
title: Beheben von DKIM-Setupproblemen
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 1389
ms.date: 04/21/2020
ms.openlocfilehash: 7bc81af961be04c8ceb1d609031042cf45da5000
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66390423"
---
# <a name="fix-dkim-setup-issues"></a>Beheben von DKIM-Setupproblemen

Wenn beim Aktivieren von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:

- Die meisten DKIM-Setupprobleme beziehen sich auf falsche DNS-Einträge. Überprüfen Sie, ob der DKIM CNAME-Eintrag (**kein** TXT-Eintrag) richtig formatiert ist. Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge verteilt werden.

- Wenn Sie die DKIM-DNS-Einträge im Admin Center nicht erstellen können, können Sie sie durch Ihre benutzerdefinierte Domäne (z. B. contoso.com) ersetzen \<CustomDomain\> und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) ausführen: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
