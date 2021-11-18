---
title: Legacyendpunkt für SMTP AUTH
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
- "3000003"
- "15320"
ms.openlocfilehash: 274b15320ae9f5ff535395427618dd2c0db735b9
ms.sourcegitcommit: 9209e36093fe5fa44663098b2a761196105e4d31
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2021
ms.locfileid: "61058863"
---
# <a name="legacy-endpoint-for-smtp-auth"></a>Legacyendpunkt für SMTP AUTH

**Wichtig:** Ein neuer Opt-In-Endpunkt ist für SMTP AUTH-Clients verfügbar, die weiterhin tls-Legacy verwenden müssen.

Obwohl die vollständige Veraltetkeit Anfang 2022 beginnt, hat Microsoft damit begonnen, einen kleinen Prozentsatz der Verbindungen abzulehnen, die TLS 1.0 für SMTP AUTH verwenden. Die Fehler sind:

- 421 4.7.66 TLS 1.0 und 1.1 werden nicht unterstützt. Aktualisieren Sie Ihren Client, um TLS 1.2 zu unterstützen.
- 5.7.67 TLS 1.0 und 1.1 werden von Ihrer Organisation nicht unterstützt.

Wenn Sie TLS 1.0/1.1 verwenden und Legacyclients, die eine Verbindung mit TLS 1.0/1.1 herstellen, beibehalten müssen, müssen Sie sich wie folgt anmelden:

- Setting the **AllowLegacyTLSClients** parameter on the Set-TransportConfig cmdlet to **True**.
- Konfigurieren von Legacyclients und -geräten für die Übermittlung an den neuen Endpunkt: "smtp-legacy.office365.com".

Weitere Informationen finden Sie unter [Neuer Opt-In-Endpunkt, der für SMTP AUTH-Clients verfügbar ist, die weiterhin tls-Legacy benötigen.](https://techcommunity.microsoft.com/t5/exchange-team-blog/new-opt-in-endpoint-available-for-smtp-auth-clients-still/ba-p/2659652)
