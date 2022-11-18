---
title: Blockieren oder Aufheben der Blockierung der externen automatischen E-Mail-Weiterleitung
ms.author: chrisda
author: chrisda
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200004"
- "726"
ms.date: 04/21/2020
ms.openlocfilehash: 7330e65da99632c532a91ae9d4c4a68f0da29d2e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66343893"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blockieren oder Aufheben der Blockierung der ewigen automatischen E-Mail-Weiterleitung

Informationen zum Aktivieren oder Deaktivieren der E-Mail-Weiterleitung für ein bestimmtes Postfach finden [Sie unter Konfigurieren der E-Mail-Weiterleitung](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Administratoren können die externe Weiterleitung für die Organisation mithilfe [von ausgehenden Spamrichtlinien](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) steuern. Sie verwalten ausgehende Spamrichtlinien im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/antispam> oder mithilfe des Cmdlets ["Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)" in Exchange Online PowerShell.

Wenn die folgende Fehlermeldung angezeigt wird: **"550 5.7.520 Zugriff verweigert, Ihre Organisation lässt externe Weiterleitung nicht zu"**, stellen Sie sicher, dass die Richtlinie so konfiguriert ist, dass externe automatisch weitergeleitete Nachrichten aktiviert sind.

**Hinweis**: Wir empfehlen den Standardwert **Automatic – System controlled** for the **Automatic forwarding rules** setting in your default outbound spam filter policy (automatic external forwarding is blocked; internal automatic forwarding still works). Sie sollten benutzerdefinierte richtlinien für ausgehende Spamfilter erstellen und den Wert **"Ein" verwenden. Die Weiterleitung ist** nur für Benutzer aktiviert, die eine externe automatische E-Mail-Weiterleitung benötigen. Weitere Informationen finden Sie [unter Konfigurieren der externen E-Mail-Weiterleitung in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
