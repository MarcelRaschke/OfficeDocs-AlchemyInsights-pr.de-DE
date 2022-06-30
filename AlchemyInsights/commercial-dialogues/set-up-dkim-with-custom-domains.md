---
title: Einrichten von DKIM mit benutzerdefinierten Domänen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002531"
- "7375"
ms.date: 02/22/2021
ms.openlocfilehash: 512e5864bd7a1194a87bdb9ccede24174ffdfec7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66356871"
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
**Hinweis**: **DomainGUID** ist der Text links von **.mail.protection.outlook.com** im angepassten MX-Eintrag für die benutzerdefinierte Domäne (z. B. contoso-com für die Domäne **contoso.com**). **InitialDomain** ist die Domäne, die Sie bei der Registrierung für Office 365 verwendet haben (z. B **. contoso.onmicrosoft.com**).

Weitere Informationen zu DNS-Einträgen finden [Sie unter Erstellen von DNS-Einträgen bei einem beliebigen DNS-Hostinganbieter für Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).