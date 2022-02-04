---
title: 'DANE- und DNSSEC-Unterstützung für Office 365 '
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9010292"
- "16312"
ms.date: 01/13/2022
ms.openlocfilehash: 62e9271ab48265ada8bbd00cfd6bb9b9d2a8efa4
ms.sourcegitcommit: 81f566eac3776bc0de39b78d0285677f21ad57a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2022
ms.locfileid: "62032838"
---
# <a name="dane-and-dnssec-support-for-office-365"></a>DANE- und DNSSEC-Unterstützung für Office 365

Antworten auf häufig gestellte Fragen:

- Die Unterstützung für DANE und DNSSEC für SMTP wird in zwei Phasen bereitgestellt. Die erste Phase ist DANE und DNSSEC für ausgehende E-Mails.
- Die zweite Phase, die Unterstützung für eingehende E-Mails, wird voraussichtlich bis Ende 2022 aktiviert sein.
- Änderungen sind standardmäßig aktiviert. Exchange Online Kunden müssen nichts tun, um diese erweiterte E-Mail-Sicherheit für ausgehende E-Mails zu konfigurieren.
- Sie können dieses Feature für einen Mandanten nicht explizit deaktivieren.
- Wenn Sie E-Mails an eine Zieldomäne senden, die DNSSEC und DANE nicht implementiert hat, werden Ihre ausgehenden E-Mails mithilfe von Opportunistic TLS gesendet.
