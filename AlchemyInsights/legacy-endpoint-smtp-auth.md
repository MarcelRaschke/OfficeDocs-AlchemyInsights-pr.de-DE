---
title: Legacyendpunkt für SMTP AUTH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3000003"
- "15320"
ms.openlocfilehash: 5cd85f5e651952d8bddff3e5fff4cb6ea00ff263
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66366793"
---
# <a name="legacy-endpoint-for-smtp-auth"></a>Legacyendpunkt für SMTP AUTH

**Wichtig**: Ein neuer Opt-In-Endpunkt steht für SMTP-AUTH-Clients zur Verfügung, die noch ältere TLS verwenden müssen.Important: A new opt-in endpoint is available for SMTP AUTH clients that still need to use legacy TLS.

Obwohl die vollständige Einstellung Anfang 2022 beginnt, hat Microsoft begonnen, einen kleinen Prozentsatz von Verbindungen abzulehnen, die TLS 1.0 für SMTP AUTH verwenden. Die Fehler lauten wie folgt:

- 421 4.7.66 TLS 1.0 und 1.1 werden nicht unterstützt. Aktualisieren Sie Ihren Client, um TLS 1.2 zu unterstützen.
- 5.7.67 TLS 1.0 und 1.1 werden von Ihrer Organisation nicht unterstützt.

Wenn Sie TLS 1.0/1.1 verwenden und Legacyclients beibehalten müssen, die eine Verbindung mit TLS1.0/1.1 herstellen, müssen Sie folgendes anmelden:

- Festlegen des **Parameters AllowLegacyTLSClients** für das cmdlet Set-TransportConfig auf **"True"**.
- Konfigurieren älterer Clients und Geräte für die Übermittlung an den neuen Endpunkt: "smtp-legacy.office365.com".

Weitere Informationen finden Sie [unter Neuer Opt-In-Endpunkt, der für SMTP-AUTH-Clients verfügbar ist, die noch ältere TLS benötigen](https://techcommunity.microsoft.com/t5/exchange-team-blog/new-opt-in-endpoint-available-for-smtp-auth-clients-still/ba-p/2659652).
