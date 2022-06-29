---
title: TLS 1.2-Verwendung für die Direct Routing-SIP-Schnittstelle erforderlich
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000321"
- "15515"
ms.openlocfilehash: 87ec54f97050cf2f0deb46043c17d6097f6769a6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66290467"
---
# <a name="tls-12-usage-required-for-the-direct-routing-sip-interface"></a>TLS 1.2-Verwendung für die Direct Routing-SIP-Schnittstelle erforderlich

Die Benachrichtigung im Nachrichtencenter nach MC297438 gilt nur für Kunden, die Direct Routing in Teams mithilfe eines Session Border Controller (SBC) und eines SIP-Proxys implementiert haben. Wenn Sie Direct Routing in Teams nicht konfiguriert haben und nicht über einen lokalen Session Border Controller verfügen, gilt dieser Beitrag im Nachrichtencenter nicht für Sie.

Wenn Sie einen lokalen SBC verwenden, stellen Sie sicher, dass Ihre SBCs für die Unterstützung von TLS 1.2 konfiguriert sind und eine Verbindung über eine der unterstützten Verschlüsselungssammlungen herstellen können.

Weitere Informationen finden Sie unter Tipps zum Konfigurieren von TLS 1.2- und Verschlüsselungssammlungen in [Windows 10](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#windows-10) oder in [Windows 8, Windows 7 oder Windows Server 2012/2008 R2(SP1)](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#windows-8-windows-7-or-windows-server-20122008-r2sp1).

Weitere Informationen zum Vorbereiten von TLS 1.2 in Office 365 finden Sie unter [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
