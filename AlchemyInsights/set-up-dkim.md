---
title: Schritte zum Einrichten von DKIM in Office 365
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3100029"
- "17477"
ms.date: 05/27/2022
ms.openlocfilehash: c4b6ee244c9b9efea66e0c345753e09642601cbe
ms.sourcegitcommit: d61bf76fd5b9f93beef0acc6a244e40258112b9b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/27/2022
ms.locfileid: "65758661"
---
# <a name="steps-to-set-up-dkim-in-office-365"></a>Schritte zum Einrichten von DKIM in Office 365

1. Für jede benutzerdefinierte Domäne, für die Sie eine DKIM-Signatur in DNS hinzufügen möchten, müssen Sie zwei CNAME-Einträge veröffentlichen. 

    Wenn Sie beispielsweise zwei benutzerdefinierte Domänen (contoso.com und fourthcoffee.com) besitzen und für beide eine DKIM-Signatur hinzufügen möchten, müssen Sie vier CNAME-Einträge veröffentlichen (zwei für contoso.com und zwei für fourthcoffee.com).

    **Hinweis**: DNS-Einträge werden innerhalb Ihrer Domänenregistrierungsstelle (dem Unternehmen, bei dem Sie Ihren Domänennamen erworben haben) verwaltet.

    Verwenden Sie dieses Format für die CNAME-Einträge für jede benutzerdefinierte Domäne:

    Hostname: `selector1._domainkey.<domain>`

    Verweist auf Adresse oder Wert: `selector1-<domainGUID>._domainkey.<initialDomain>`

    TTL: 3600

    Hostname: `selector2._domainkey.<domain>`

    Verweist auf Adresse oder Wert: `selector2-<domainGUID>._domainkey.<initialDomain>`

    TTL: 3600

    Beispiel: Wenn Ihre benutzerdefinierte Domäne contoso.com ist und Ihre ursprüngliche Domäne contosocompany.onmicrosoft.com ist, sehen die CNAME-Einträge wie folgt aus:

    Hostname: `selector1._domainkey.contoso.com`

    Verweist auf Adresse oder Wert: `selector1-contoso-com._domainkey. contosocompany.onmicrosoft.com`

    TTL: 3600

    Hostname: `selector2._domainkey.contoso.com`

    Verweist auf Adresse oder Wert: `selector2-contoso-com._domainkey. contosocompany.onmicrosoft.com`

    TTL: 3600

    Wiederholen Sie diesen Schritt für jede benutzerdefinierte Domäne.

2. Nachdem Sie Ihre CNAME-Einträge im DNS veröffentlicht haben, schließen Sie das DKIM-Setup ab:

    Melden Sie sich mit Ihrem Geschäfts-, Schul- oder Unikonto bei Office 365 an, und wechseln **Sie zu Sicherheitsrichtlinien (Microsoft 365 Defender)** >  **& Regeln** > **Bedrohungsrichtlinien** > **DomainKeys Identified Mail (DKIM)**.

Weitere Informationen finden Sie unter [Verwenden von DKIM zum Überprüfen ausgehender E-Mails, die von Ihrer benutzerdefinierten Domäne gesendet wurden](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#how-dkim-works-better-than-spf-alone-to-prevent-malicious-spoofing-in-office-365).

