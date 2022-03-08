---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 965b8af22a4c8dfd9b1a406726047ff7ee0ee653
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63095842"
---
# <a name="alert-policies"></a>Warnungsrichtlinien

Microsoft 365 enthält [Standardwarnungsrichtlinien](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies), die Warnungen für Organisationen mit einem Microsoft 365 Enterprise- oder Microsoft 365 US Government E1/G1-, E3/G3- oder E5/G5-Abonnement auslösen. Daher erhalten Administratoren möglicherweise eine Benachrichtigung per E-Mail, die von Office365Alerts@microsoft.com mit einer Betreffzeile wie "Warnung mit niedriger Dringlichkeit: *Name der Warnungsrichtlinie*" gesendet wird. Warnungsbenachrichtigungen werden gesendet, wenn Warnungen für allgemeine Aktivitäten ausgelöst werden, z. B. wenn Benutzer:

- Erstellen Sie Posteingangsregeln, die E-Mails weiterleiten.
- Weisen Sie Berechtigungen für ihr Postfach zu.
- Freigeben oder Löschen einer großen Anzahl von Dateien in SharePoint Dateifreigabe.
- Erstellen sie eDiscovery-Suchvorgänge, und exportieren Sie Suchergebnisse.

So überprüfen Und reagieren Sie auf eine Warnung:

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com>zu **"Warnungen"**. Oder verwenden Sie , um direkt zur Seite **"Warnungen** " zu wechseln <https://compliance.microsoft.com/compliancealerts>.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com>zu **"Vorfälle & Warnungen** \> **"**. Oder verwenden Sie , um direkt zur Seite **"Warnungen** " zu wechseln <https://security.microsoft.com/alerts>.
2. Klicken Sie auf eine Warnung, um eine Flyoutseite mit Informationen zu der Warnung anzuzeigen.

Sie können Maßnahmen für eine Warnung ergreifen, z. B. [das Entfernen einer verdächtigen Posteingangsregel](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Sie können die Warnung auch einfach schließen, indem Sie auf der Flyoutseite der Warnung auf **"Auflösen** " klicken.

Weitere Informationen zum Konfigurieren und Verwalten von Warnungsrichtlinien finden Sie in  [diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**Wichtig**: Benachrichtigungen über E-Mail-Benachrichtigungen von Microsoft werden Sie niemals bitten, Folgendes zu tun:

- Bereitstellen eines Kennworts
- Überprüfen der Sicherheitsdetails Ihres Kontos
- Sich selbst erneut authentifizieren

Wenn Sie eine E-Mail-Nachricht mit diesen Arten von Anforderungen erhalten, wurde sie nicht von Microsoft gesendet und sollte als Phishing-Betrug betrachtet werden. Wenn Sie eine Nachricht mit diesen Arten von Anforderungen erhalten, [melden Sie die Nachricht an Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
