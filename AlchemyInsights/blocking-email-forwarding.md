---
title: Blockieren oder Aufheben der Blockierung der automatischen externen E-Mail-Weiterleitung
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 63cbd26f5fd43411b88f7fc1302915797c287fc2
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63258785"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blockieren oder Aufheben der Blockierung der automatischen E-Mail-Weiterleitung

Informationen zum Aktivieren oder Deaktivieren der E-Mail-Weiterleitung für ein bestimmtes Postfach finden Sie unter [Konfigurieren der E-Mail-Weiterleitung](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Administratoren können die externe Weiterleitung für die Organisation mithilfe [ausgehender Spamrichtlinien](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) steuern. Sie verwalten ausgehende Spamrichtlinien im Microsoft 365 Defender Portal unter <https://security.microsoft.com/antispam> oder mithilfe des Cmdlets ["Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)" in Exchange Online PowerShell.

Wenn die folgende Fehlermeldung angezeigt wird: **"550 5.7.520 Zugriff verweigert, Ihre Organisation lässt keine externe Weiterleitung zu"**, stellen Sie sicher, dass die Richtlinie so konfiguriert ist, dass externe automatisch weitergeleitete Nachrichten aktiviert werden.

**Hinweis**: Wir empfehlen den Standardwert **"Automatisch– System gesteuert** für die Einstellung für die **automatische Weiterleitungsregeln** " in Ihrer standardmäßigen Richtlinie für ausgehende Spamfilter (die automatische externe Weiterleitung wird blockiert; die interne automatische Weiterleitung funktioniert weiterhin). Sie sollten benutzerdefinierte richtlinien für ausgehende Spamfilter erstellen und den Wert **"Ein – Weiterleitung"** nur für Benutzer verwenden, die eine externe automatische E-Mail-Weiterleitung benötigen. Weitere Informationen finden Sie unter [Konfigurieren der externen E-Mail-Weiterleitung in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
