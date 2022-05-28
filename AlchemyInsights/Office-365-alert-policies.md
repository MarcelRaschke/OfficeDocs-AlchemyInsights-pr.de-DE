---
title: 1385-Office-365-alert-policies
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3200002"
- "1385"
ms.openlocfilehash: 4e6955127abd2bb320d23b99163c6283378ab250
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65723108"
---
# <a name="alert-policies"></a>Warnungsrichtlinien

Microsoft 365 enthält [Standardwarnungsrichtlinien](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies), die Warnungen für Organisationen mit einem Microsoft 365 Enterprise- oder Microsoft 365 US Government E1/G1-, E3/G3- oder E5/G5-Abonnement auslösen. Administratoren erhalten daher möglicherweise eine von Office365Alerts@microsoft.com gesendete E-Mail-Benachrichtigung mit einer Betreffzeile wie "Warnung mit niedrigem Schweregrad: *Name der Warnungsrichtlinie*". Warnungsbenachrichtigungen werden gesendet, wenn Warnungen für allgemeine Aktivitäten ausgelöst werden, z. B. wenn Benutzer:

- Erstellen Sie Posteingangsregeln, die E-Mails weiterleiten.
- Weisen Sie ihrem Postfach Berechtigungen zu.
- Freigeben oder Löschen einer großen Anzahl von Dateien in SharePoint Dateifreigabe.
- Erstellen Sie eDiscovery-Suchvorgänge, und exportieren Sie Suchergebnisse.

So überprüfen Und reagieren Sie auf eine Warnung:

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie in der Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com>zu **"Benachrichtigungen"**. Oder verwenden Sie <https://compliance.microsoft.com/compliancealerts>, um direkt zur Seite "**Warnungen**" zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender Portal unter <https://security.microsoft.com>zu **"Vorfälle & Warnungen**\>". Oder verwenden Sie <https://security.microsoft.com/alerts>, um direkt zur Seite "**Warnungen**" zu wechseln.
2. Klicken Sie auf eine Warnung, um eine Flyoutseite mit Informationen zu der Warnung anzuzeigen.

Sie können Maßnahmen für eine Warnung ergreifen, z. [B. eine verdächtige Posteingangsregel entfernen](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Oder Sie können die Benachrichtigung einfach schließen, indem Sie auf der Flyoutseite der Warnung auf **"Auflösen** " klicken.

Weitere Informationen zum Konfigurieren und Verwalten von Warnungsrichtlinien finden Sie  [in diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**Wichtig**: Benachrichtigungs-E-Mail-Benachrichtigungen von Microsoft werden Sie niemals bitten, Folgendes zu tun:

- Angeben eines Kennworts
- Überprüfen der Sicherheitsdetails Ihres Kontos
- Erneute Authentifizierung

Wenn Sie eine E-Mail-Nachricht mit diesen Arten von Anforderungen erhalten, wurde sie nicht von Microsoft gesendet und sollte als Phishing-Betrug angesehen werden. Wenn Sie eine Nachricht mit diesen Arten von Anforderungen erhalten, [melden Sie die Nachricht an Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
