---
title: TLS 1.2-Verwendung erforderlich für die Direct Routing-SIP-Schnittstelle
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000321"
- "15515"
ms.openlocfilehash: 695fb10d4ee0a744f0efdf811162c29375252c11
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63189608"
---
# <a name="tls-12-usage-required-for-the-direct-routing-sip-interface"></a>TLS 1.2-Verwendung erforderlich für die Direct Routing-SIP-Schnittstelle

Die Benachrichtigung im Nachrichtencenter nach MC297438 gilt nur für Kunden, die Direct Routing in Teams mithilfe eines Session Border Controllers (SBC) und eines SIP-Proxys implementiert haben. Wenn Sie Direct Routing in Teams nicht konfiguriert haben und keinen lokalen Session Border Controller haben, gilt dieser Nachrichtencenterbeitrag nicht für Sie.

Wenn Sie einen lokalen SBC verwenden, stellen Sie sicher, dass Ihre SBCs für die Unterstützung von TLS 1.2 konfiguriert sind und eine Verbindung mithilfe einer der unterstützten Verschlüsselungssammlungen herstellen können.

Weitere Informationen finden Sie unter Tipps zum Konfigurieren von TLS 1.2 und Verschlüsselungssammlungen in [Windows 10](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#windows-10) oder in [Windows 8, Windows 7 oder Windows Server 2012/2008 R2(SP1)](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#windows-8-windows-7-or-windows-server-20122008-r2sp1).

Weitere Informationen zum Vorbereiten von TLS 1.2 in Office 365 finden Sie unter [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
