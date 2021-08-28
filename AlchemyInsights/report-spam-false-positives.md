---
title: Möchten Sie Microsoft ein falsch positives Spam melden?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396614"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Werden zulässige Nachrichten als Spam gekennzeichnet?

Es ist frustrierend, wenn eine seriöse E-Mail im Junk-Ordner oder in Quarantäne endet. Berücksichtigen Sie die häufigsten Gründe für falsch positive Ergebnisse:

**Mandantenüberschreibungen (am häufigsten)** Dies liegt vollständig in Ihrem Steuerelement, um Abhilfe zu suchen.

Senden Sie die Nachricht über Microsoft 365 Defender zur Analyse der auswirkungenden Richtlinien und Regeln; Details zum erneuten Scannen sind innerhalb von Minuten verfügbar.
Überprüfen oder ändern Sie ggf. die Richtlinien oder Regeln. 

**Außerkraftsetzungen für Endbenutzer (allgemein)** Dies liegt vollständig in Ihrem Steuerelement, um Abhilfe zu suchen. 

Senden Sie die Nachricht über Microsoft 365 Defender zur Analyse der auswirkungenden Richtlinien und Regeln; Details zum erneuten Scannen sind innerhalb von Minuten verfügbar. 

Wenn eine Nachricht blockiert wurde, weil sie von einer Adresse in der Liste blockierter Absender eines Benutzers gesendet wurde, enthalten die Kopfzeilen die Spamfilterbewertung "SFV:BLK".

**E-Mail-Authentifizierung von Absendern** Dies liegt teilweise innerhalb Ihres Steuerelements, um dies zu beheben.

Senden Sie die Nachricht, um Fehler in der E-Mail-Authentifizierung des Absenders zum Zeitpunkt der Zustellung zu analysieren. Die Ergebnisse sind innerhalb eines Tages verfügbar. 

Wenn Sie Besitzer der sendenden Infrastruktur sind, überprüfen Sie, wie Sie sie an SPF, DKIM und DMARC ausrichten, um sicherzustellen, dass Ziel-E-Mail-Systeme Nachrichten vertrauen, die von Ihrer Domäne gesendet werden. Alternativ können Sie sich an die Absender wenden, um ihre DNS-Konfigurationen zu adressieren.

**Microsoft-Filterbewertungen** Dies liegt teilweise innerhalb Ihres Steuerelements, um dies zu beheben.

Senden Sie die Nachricht, und melden Sie die Nachricht als sicher. Ergebnisse des erneuten Scannens sind innerhalb eines Tages verfügbar. Verwenden Sie die Mandanten-Zulassungs-/Sperrliste, wenn Sie mit Filterbewertungen in bestimmten Situationen nicht einverstanden sind. Sie sollten die Microsoft-Filterbewertungen jedoch nicht dauerhaft umgehen. 

Weitere Informationen finden Sie unter:

- Ermöglichen Sie Ihren Endbenutzern, Nachrichten an Microsoft zu übermitteln. Microsoft verwendet diese Übermittlungen, um die Effektivität von E-Mail-Schutztechnologien zu verbessern, und sie werden in Übermittlungsberichten angezeigt, die Sie als Hinweise zum Aktualisieren von Richtlinien verwenden können. 

- Ein kurzes Video zum Übermitteln von Nachrichten zur Analyse finden Sie unter ["Übermitteln von Nachrichten für die Analyse".](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Verwenden von Administrator-Übermittlung, um verdächtige Spam- oder Phishing-Nachrichten, URLs und Dateien an Microsoft zu übermitteln](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Verwalten der Zulassungs-/Sperrliste des Mandanten](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Antispam-Nachrichtenkopfzeilen in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Schutz vor ausgehenden Spamnachrichten in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)