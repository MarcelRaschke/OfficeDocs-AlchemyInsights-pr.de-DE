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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332306"
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
**Hinweis:** **DomainGUID** ist der Text links von **.mail.protection.outlook.com** im angepassten MX-Eintrag für die benutzerdefinierte Domäne (z. B. contoso-com für die Domäne **contoso.com**). **InitialDomain** ist die Domäne, die Sie bei der Registrierung für Office 365 (z. **B. contoso.onmicrosoft.com)** verwendet haben.

Weitere Informationen zu DNS-Einträgen finden Sie unter [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).