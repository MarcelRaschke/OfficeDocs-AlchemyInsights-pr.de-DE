---
title: 'DANE- und DNSSEC-Unterstützung für Office 365 '
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010292"
- "16312"
ms.date: 08/16/2022
ms.openlocfilehash: 9a5ec9893212ef4b5f62b10663f371b606ea0b1f
ms.sourcegitcommit: 7acf85b81ce9e2975e2fddfe6d674a51643bffa7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/29/2022
ms.locfileid: "67453497"
---
# <a name="dane-and-dnssec-support-for-office-365"></a>DANE- und DNSSEC-Unterstützung für Office 365

Antworten auf häufig gestellte Fragen:

- Die Unterstützung für DANE und DNSSEC für SMTP wird in zwei Phasen bereitgestellt. Die erste Phase ist DANE und DNSSEC für ausgehende E-Mails.
- Die zweite Phase, die Unterstützung für eingehende E-Mails, wird voraussichtlich Ende 2022 aktiviert sein.
- Änderungen sind standardmäßig aktiviert. Exchange Online Kunden müssen nichts tun, um diese erweiterte E-Mail-Sicherheit für ausgehende E-Mails zu konfigurieren.
- Sie können dieses Feature für einen Mandanten nicht explizit deaktivieren.
- Wenn Sie E-Mails an eine Zieldomäne senden, die DNSSEC und DANE nicht implementiert hat, werden Ihre ausgehenden E-Mails mit Opportunistic TLS gesendet.
