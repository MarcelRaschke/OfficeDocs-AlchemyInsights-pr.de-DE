---
title: Einrichten von DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 443e69d4f81a46f5decd03566f3511fb1aa9fab1
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63293131"
---
# <a name="setup-dkim"></a>Einrichten von DKIM

Die vollständigen Anweisungen zum Konfigurieren von DKIM für benutzerdefinierte Domänen in Microsoft 365 finden Sie [hier](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Für **jede** benutzerdefinierte Domäne müssen Sie **zwei** DKIM CNAME-Einträge beim DNS-Hostingdienst Ihrer Domäne erstellen (in der Regel die Domänenregistrierungsstelle). Beispielsweise erfordern contoso.com und fourthcoffee.com vier DKIM-CNAME-Einträge: zwei für contoso.com und zwei für fourthcoffee.com.

   Die DKIM CNAME-Einträge für **jede** benutzerdefinierte Domäne verwenden die folgenden Formate:

   - **Hostname**: `selector1._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostname**: `selector2._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> ist der Text links neben dem benutzerdefinierten `.mail.protection.outlook.com` MX-Eintrag für die benutzerdefinierte Domäne (z `contoso-com` . B. für die Domäne contoso.com). \<InitialDomain\>ist die Domäne, die Sie bei der Registrierung für Microsoft 365 verwendet haben (z. B. contoso.onmicrosoft.com).

2. Nachdem Sie die CNAME-Einträge für Ihre benutzerdefinierten Domänen erstellt haben, führen Sie die folgenden Anweisungen aus:

   a. [melden Sie sich](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) mit Ihrem Geschäfts-, Schul- oder Unikonto bei Microsoft 365 an.

   b. Klicken Sie oben links auf das App-Startsymbol, und wählen Sie **Admin** aus.

   c. Erweitern Sie im unteren linken Navigationsbereich **Admin**, und klicken Sie dann auf **Exchange**.

   d. Wechseln Sie zu **"****ProtectionDKIM** > ".

   e. Wählen Sie die Domäne aus, und wählen Sie dann "Zum **Signieren von Nachrichten für diese Domäne mit DKIM-Signaturen** **aktivieren**" aus. Wiederholen Sie diesen Schritt für jede benutzerdefinierte Domäne.
