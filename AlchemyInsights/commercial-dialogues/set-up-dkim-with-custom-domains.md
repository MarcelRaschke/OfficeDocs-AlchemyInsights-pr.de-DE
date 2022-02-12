---
title: Einrichten von DKIM mit benutzerdefinierten Domänen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 09f06ceb8b1cfe87b30d393e909a71f83e82eb98
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62687588"
---
# <a name="set-up-dkim-with-custom-domains"></a>Einrichten von DKIM mit benutzerdefinierten Domänen

Sie müssen zwei CNAME-Einträge für jede benutzerdefinierte Domäne in DNS veröffentlichen. Verwenden Sie dazu das folgende Format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Hinweis**: **DomainGUID** ist der Text links von **.mail.protection.outlook.com** im angepassten MX-Eintrag für die benutzerdefinierte Domäne (z. B. contoso-com für die Domäne **contoso.com**). **InitialDomain** ist die Domäne, die Sie bei der Registrierung für Office 365 verwendet haben (z. **B. contoso.onmicrosoft.com**).

Weitere Informationen zu DNS-Einträgen finden [Sie unter Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).