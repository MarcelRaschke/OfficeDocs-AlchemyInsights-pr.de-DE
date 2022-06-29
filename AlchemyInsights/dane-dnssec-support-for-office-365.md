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
ms.date: 01/13/2022
ms.openlocfilehash: 048ef3d2b7d803ce5eaa53add424ef3c72b79c4e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66354855"
---
# <a name="dane-and-dnssec-support-for-office-365"></a>DANE- und DNSSEC-Unterstützung für Office 365

Antworten auf häufig gestellte Fragen:

- Die Unterstützung für DANE und DNSSEC für SMTP wird in zwei Phasen bereitgestellt. Die erste Phase ist DANE und DNSSEC für ausgehende E-Mails.
- Die zweite Phase, die Unterstützung für eingehende E-Mails, wird voraussichtlich Ende 2022 aktiviert sein.
- Änderungen sind standardmäßig aktiviert. Exchange Online Kunden müssen nichts tun, um diese erweiterte E-Mail-Sicherheit für ausgehende E-Mails zu konfigurieren.
- Sie können dieses Feature für einen Mandanten nicht explizit deaktivieren.
- Wenn Sie E-Mails an eine Zieldomäne senden, die DNSSEC und DANE nicht implementiert hat, werden Ihre ausgehenden E-Mails mit Opportunistic TLS gesendet.
