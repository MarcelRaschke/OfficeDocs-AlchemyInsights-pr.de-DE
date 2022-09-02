---
title: 550 5.7.1 Mindestens ein Empfänger wird durch die Blockierungsrichtlinie für Mandantenempfänger Ihrer Organisation blockiert.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200009"
- "18179"
ms.openlocfilehash: ee129114ba6e7fffcca036d926b570df91fc2b22
ms.sourcegitcommit: 7c650f8e0593bbb15db359384b89550a35ab7707
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/02/2022
ms.locfileid: "67571935"
---
# <a name="550-571-one-or-more-recipients-are-blocked-by-your-organizations-tenant-recipient-block-policy"></a>550 5.7.1 Mindestens ein Empfänger wird durch die Blockierungsrichtlinie für Mandantenempfänger Ihrer Organisation blockiert.

Wenn Sie die Meldung "550 5.7.1 Ihre Nachricht kann nicht zugestellt werden, weil ein oder mehrere Empfänger durch die Mandantenempfänger-Sperrrichtlinie AS(8910)" Ihrer Organisation blockiert werden, ist die E-Mail-Adresse oder Domäne eines der Empfänger Teil der blockierten Domänen und Adressen in der **Mandanten-Zulassungs-/Sperrliste** Ihrer Organisation. Um dies zu beheben, überprüfen und entfernen Sie den entsprechenden Eintrag.

Weitere Informationen finden Sie unter:

- [Beheben von Problemen bei der E-Mail-Zustellung für Fehlercode 550 5.7.1 in Exchange Online](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-550-5-7-1-in-exchange-online#im-an-email-admin-how-can-i-fix-this-issue)
- [Zulassen oder Blockieren von E-Mails mithilfe der Mandanten-Zulassungs-/Sperrliste](https://docs.microsoft.com/microsoft-365/security/office-365-security/allow-block-email-spoof#use-the-microsoft-365-defender-portal-to-remove-allow-or-block-entries-for-domains-and-email-addresses-in-the-tenant-allowblock-list).