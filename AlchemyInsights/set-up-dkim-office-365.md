---
title: Einrichten von DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108555"
---
# <a name="setup-dkim"></a>Einrichten von DKIM

Die vollständigen Anweisungen zum Konfigurieren von DKIM für benutzerdefinierte Domänen in Microsoft 365 finden Sie [hier.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Für **jede** benutzerdefinierte Domäne müssen Sie **zwei** DKIM CNAME-Einträge beim DNS-Hostingdienst Ihrer Domäne erstellen (in der Regel die Domänenregistrierungsstelle). Beispielsweise erfordern contoso.com und fourthcoffee.com vier DKIM-CNAME-Einträge: zwei für contoso.com und zwei für fourthcoffee.com.

   Die DKIM CNAME-Einträge für **jede** benutzerdefinierte Domäne verwenden die folgenden Formate:

   - **Hostname:**`selector1._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostname:**`selector2._domainkey.<CustomDomain>`

     **Verweist auf Adresse oder Wert:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> ist der Text links neben `.mail.protection.outlook.com` dem angepassten MX-Eintrag für die benutzerdefinierte Domäne (z. `contoso-com` B. für die Domäne contoso.com). \<InitialDomain\>ist die Domäne, die Sie bei der Registrierung für Microsoft 365 verwendet haben (z. B. contoso.onmicrosoft.com).

2. Nachdem Sie die CNAME-Einträge für Ihre benutzerdefinierten Domänen erstellt haben, führen Sie die folgenden Anweisungen aus:

   a. [melden Sie sich](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) mit Ihrem Geschäfts-, Schul- oder Unikonto bei Microsoft 365 an.

   b. Klicken Sie oben links auf das App-Startsymbol, und wählen Sie **Admin** aus.

   c. Erweitern Sie im unteren linken Navigationsbereich **Admin**, und klicken Sie dann auf **Exchange**.

   d. Wechseln Sie zu **"Schutz**  >  **DKIM".**

   e. Wählen Sie die Domäne aus, und wählen Sie dann **"Zum Signieren von Nachrichten für diese Domäne mit DKIM-Signaturen** **aktivieren"** aus. Wiederholen Sie diesen Schritt für jede benutzerdefinierte Domäne.
