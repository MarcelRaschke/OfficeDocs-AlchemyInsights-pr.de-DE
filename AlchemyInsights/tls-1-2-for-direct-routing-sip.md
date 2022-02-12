---
title: TLS 1.2-Verwendung erforderlich für die Direct Routing-SIP-Schnittstelle
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
- "9000321"
- "15515"
ms.openlocfilehash: 295206b4c6f12646a6d332d62174a8f974878563
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62676368"
---
# <a name="tls-12-usage-required-for-the-direct-routing-sip-interface"></a>TLS 1.2-Verwendung erforderlich für die Direct Routing-SIP-Schnittstelle

Die Benachrichtigung im Nachrichtencenter nach MC297438 gilt nur für Kunden, die Direct Routing in Teams mithilfe eines Session Border Controller (SBC) und eines SIP-Proxys implementiert haben. Wenn Sie Direct Routing in Teams nicht konfiguriert haben und keinen lokalen Session Border Controller haben, gilt dieser Nachrichtencenterbeitrag nicht für Sie.

Wenn Sie einen lokalen SBC verwenden, stellen Sie sicher, dass Ihre SBCs für die Unterstützung von TLS 1.2 konfiguriert sind und eine Verbindung mithilfe einer der unterstützten Verschlüsselungssammlungen herstellen können.

Weitere Informationen finden Sie unter Tipps zum Konfigurieren von TLS 1.2 und Verschlüsselungssammlungen in [Windows 10](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#windows-10) oder in [Windows 8, Windows 7 oder Windows Server 2012/2008 R2(SP1)](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#windows-8-windows-7-or-windows-server-20122008-r2sp1).

Weitere Informationen zum Vorbereiten von TLS 1.2 in Office 365 finden Sie unter [Vorbereiten für TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
