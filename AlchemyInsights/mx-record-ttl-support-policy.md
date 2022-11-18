---
title: MX-Eintrag TTL-Supportrichtlinie MC346908
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "100001"
- "17161"
ms.date: 04/12/2022
ms.openlocfilehash: cd0242ddd61cb8bc5420339a0cd6a737cfe22288
ms.sourcegitcommit: b6ba43b438551e7558ad67d8b94f84b608d26bf9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2022
ms.locfileid: "64826487"
---
# <a name="mx-record-ttl-support-policy-mc346908"></a>MX-Eintrag TTL-Supportrichtlinie MC346908

Die empfohlene TTL für MX-Einträge beträgt 1 Stunde oder 3600 Sekunden. Die maximale TTL wurde auf 6 Stunden oder 21600 Sekunden gesenkt.

So überprüfen Sie die TTL eines MX-Eintrags im Verwaltungsportal:

1. Navigieren Sie dazu zu **Einstellungen** > [Domänen](https://portal.office.com/Adminportal/Home?ref=/Domains).
2. Doppelklicken Sie auf eine benutzerdefinierte Domäne, und wählen Sie dann **DNS-Einträge** aus, um den MX-Eintrag TTL anzuzeigen.

    Die Registrierungsstelle, die Ihre Domäne verwaltet, wird oben auf der Seite unter dem Domänennamen angezeigt.

Informationen zum Ändern Ihrer DNS-Einträge, einschließlich der TTL, finden Sie unter [Ändern von DNS-Einträgen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider#step-2-add-dns-records-to-connect-microsoft-services).

Domänen, die von Microsoft- oder ONMICROSOFT-Domänen verwaltet werden, erfordern keine Aktion.

Das Senken der TTL wirkt sich nicht auf Ihren E-Mail-Dienst aus.
