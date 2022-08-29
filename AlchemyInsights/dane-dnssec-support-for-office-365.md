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
- "3200003"
- "16312"
- "13753"
ms.date: 08/16/2022
ms.openlocfilehash: 4ad2f3013ee81a8c75999b37db2e6969957c1d4f
ms.sourcegitcommit: cfb31af0138b5370c878e0801441eab1878ebf3a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/17/2022
ms.locfileid: "67364750"
---
# <a name="dane-and-dnssec-support-for-office-365"></a>DANE- und DNSSEC-Unterstützung für Office 365

Antworten auf häufig gestellte Fragen:

- Die Unterstützung für DANE und DNSSEC für SMTP wird in zwei Phasen bereitgestellt. Die erste Phase ist DANE und DNSSEC für ausgehende E-Mails.
- Die zweite Phase, die Unterstützung für eingehende E-Mails, wird voraussichtlich Ende 2022 aktiviert sein.
- Änderungen sind standardmäßig aktiviert. Exchange Online Kunden müssen nichts tun, um diese erweiterte E-Mail-Sicherheit für ausgehende E-Mails zu konfigurieren.
- Sie können dieses Feature für einen Mandanten nicht explizit deaktivieren.
- Wenn Sie E-Mails an eine Zieldomäne senden, die DNSSEC und DANE nicht implementiert hat, werden Ihre ausgehenden E-Mails mit Opportunistic TLS gesendet.
