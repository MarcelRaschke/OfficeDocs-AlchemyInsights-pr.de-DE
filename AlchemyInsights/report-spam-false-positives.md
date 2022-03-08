---
title: Möchten Sie Microsoft ein falsch positives Spam melden?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: 3fdbfc8cfe6ba75fa6b22bd309460fe5365f6775
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63085798"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Werden zulässige Nachrichten als Spam gekennzeichnet?

Es ist frustrierend, wenn eine seriöse E-Mail im Junk-Ordner oder in Quarantäne endet.

Sie können die Nachricht zur Analyse an Microsoft auf der Seite **"Übermittlungen** " im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/reportsubmission?viewid=admin>senden.

Berücksichtigen Sie die häufigsten Gründe für falsch positive Ergebnisse:

**Außerkraftsetzungen (am häufigsten):** Diese Ursache liegt _vollständig_ innerhalb Ihres Steuerelements, um Abhilfe zu suchen.

Übermitteln Sie die Nachricht zur Analyse der betroffenen Richtlinien und Regeln. Details zum erneuten Scannen sind innerhalb von Minuten verfügbar.

Überprüfen oder ändern Sie ggf. die Richtlinien oder Regeln.

**Außerkraftsetzungen von Endbenutzern (allgemein):** Diese Ursache liegt _vollständig_ in Ihrem Steuerungsbereich, um Abhilfe zu suchen.

Übermitteln Sie die Nachricht zur Analyse der betroffenen Richtlinien und Regeln. Details zum erneuten Scannen sind innerhalb von Minuten verfügbar.

Wenn eine Nachricht blockiert wurde, weil sie von einer Adresse in der Liste blockierter Absender eines Benutzers gesendet wurde, hat der [X-Forefront-Antispam-Report-Nachrichtenkopf](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers#x-forefront-antispam-report-message-header-fields) den Wert `SFV:BLK`.

**Absender-E-Mail-Authentifizierung**: Diese Ursache liegt _teilweise_ innerhalb Ihres Steuerelements, um Abhilfe zu erzielen.

Senden Sie die Nachricht, um Fehler in der E-Mail-Authentifizierung des Absenders zum Zeitpunkt der Zustellung zu analysieren. Ergebnisse sind innerhalb eines Tages verfügbar.

Wenn Sie Besitzer der sendenden Infrastruktur sind, überprüfen Sie, wie Sie sie an [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing), [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) und [DMARC](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dmarc-to-validate-email) ausrichten, um sicherzustellen, dass Ziel-E-Mail-Systeme Nachrichten vertrauen, die von Ihrer Domäne gesendet werden. Alternativ können Sie sich an die Absender wenden, um ihre DNS-Konfigurationen zu adressieren.

**Microsoft-Filterbewertungen**: Diese Ursache liegt _teilweise_ innerhalb Ihres Steuerelements, um Abhilfe zu suchen.

Senden Sie die Nachricht, und melden Sie die Nachricht als sicher. Erneutes Scannen der Ergebnisse ist innerhalb eines Tages verfügbar.

Verwenden Sie die [Mandanten-Zulassungs-/Sperrliste](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list) , wenn Sie mit Filterbewertungen in bestimmten Situationen nicht einverstanden sind. [Sie sollten microsoft-Filterbewertungen jedoch nicht dauerhaft umgehen](https://docs.microsoft.com/exchange/troubleshoot/antispam-and-protection/cautions-against-bypassing-spam-filters).

Weitere Informationen finden Sie unter:

- [Ermöglichen Sie Ihren Endbenutzern, Nachrichten an Microsoft zu übermitteln](https://docs.microsoft.com/microsoft-365/security/office-365-security/user-submission). Microsoft verwendet diese Übermittlungen, um die Effektivität von E-Mail-Schutztechnologien zu verbessern, und sie werden in Übermittlungsberichten angezeigt, die Sie als Hinweis zum Aktualisieren von Richtlinien verwenden können.
- Ein kurzes Video zum Übermitteln von Nachrichten zur Analyse finden Sie unter ["Übermitteln von Beispielen für die Analyse](https://www.youtube.com/watch?v=ta5S09Yz6Ks)".
- [Verwenden der Administratorübermittlung zum Übermitteln von verdächtigem Spam, Phishing, URLs und Dateien an Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)
- [Schutz vor ausgehenden Spamnachrichten in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)
