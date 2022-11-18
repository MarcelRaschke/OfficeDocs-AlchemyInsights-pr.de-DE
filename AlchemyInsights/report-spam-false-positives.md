---
title: Möchten Sie Microsoft ein falsch positives Spam-Ergebnis melden?
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100019"
- "975"
- "666"
ms.openlocfilehash: 6e366e45fb3dfead9815a30c3c1b83f104f514dc
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66430484"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Werden zulässige Nachrichten als Spam gekennzeichnet?

Es ist frustrierend, wenn eine legitime E-Mail im Junk-Ordner oder in Quarantäne landet.

Sie können die Nachricht zur Analyse an Microsoft auf der Seite **"Übermittlungen**" im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/reportsubmission?viewid=admin>übermitteln.

Berücksichtigen Sie die folgenden häufigsten Gründe für falsch positive Ergebnisse:

**Außerkraftsetzungen (am häufigsten):** Diese Ursache liegt _vollständig_ in Ihrem Steuerelement zur Behebung.

Senden Sie die Nachricht zur Analyse der sich auswirkenden Richtlinien und Regeln. Details zum erneuten Scannen sind innerhalb von Minuten verfügbar.

Überprüfen oder ändern Sie die Richtlinien oder Regeln nach Bedarf.

**Endbenutzerüberschreibungen (allgemein):** Diese Ursache liegt _vollständig_ in Ihrem Steuerelement zur Behebung.

Senden Sie die Nachricht zur Analyse der sich auswirkenden Richtlinien und Regeln. Details zum erneuten Scannen sind innerhalb von Minuten verfügbar.

Wenn eine Nachricht blockiert wurde, weil sie von einer Adresse in der Liste blockierter Absender eines Benutzers gesendet wurde, hat die [X-Forefront-Antispam-Report-Nachrichtenkopfzeile](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers#x-forefront-antispam-report-message-header-fields) den Wert `SFV:BLK`.

**Absender-E-Mail-Authentifizierung**: Diese Ursache liegt _teilweise_ in Ihrem Steuerelement zur Behebung.

Senden Sie die Nachricht, um Fehler in der E-Mail-Authentifizierung des Absenders zum Zeitpunkt der Zustellung zu analysieren. Ergebnisse sind innerhalb eines Tages verfügbar.

Wenn Sie die sendende Infrastruktur besitzen, überprüfen Sie, wie Sie sie an [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing), [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) und [DMARC](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dmarc-to-validate-email) ausrichten, um sicherzustellen, dass Ziel-E-Mail-Systeme Nachrichten vertrauen, die von Ihrer Domäne gesendet werden. Alternativ können Sie die Absender kontaktieren, um ihre DNS-Konfigurationen zu adressieren.

**Microsoft-Filterbewertungen**: Diese Ursache liegt _teilweise_ in Ihrem Steuerelement zur Behebung.

Senden Sie die Nachricht, und melden Sie die Nachricht als sicher. Die Ergebnisse des erneuten Scannens sind innerhalb eines Tages verfügbar.

Verwenden Sie die [Zulassungs-/Sperrliste des Mandanten](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list) , wenn Sie mit dem Filtern von Bewertungen in bestimmten Situationen nicht einverstanden sind. [Sie sollten Microsoft-Filterbewertungen jedoch nicht dauerhaft umgehen](https://docs.microsoft.com/exchange/troubleshoot/antispam-and-protection/cautions-against-bypassing-spam-filters).

Weitere Informationen finden Sie unter:

- [Ermöglichen Sie Ihren Endbenutzern das Senden von Nachrichten an Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/user-submission). Microsoft verwendet diese Übermittlungen, um die Effektivität von E-Mail-Schutztechnologien zu verbessern, und sie werden in Übermittlungsberichten angezeigt, die Sie als Hinweis zum Aktualisieren von Richtlinien verwenden können.
- Ein kurzes Video zum Senden von Nachrichten zur Analyse finden Sie unter [Übermitteln von Beispielen für die Analyse](https://www.youtube.com/watch?v=ta5S09Yz6Ks).
- [Verwenden sie Admin Übermittlung, um verdächtige Spam- und Phishing-Nachrichten, URLs und Dateien an Microsoft zu übermitteln.](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)
- [Ausgehender Spamschutz in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)
