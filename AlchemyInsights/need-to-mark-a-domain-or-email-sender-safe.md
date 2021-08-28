---
title: Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319947"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?

- Die Verwendung von **Listen sicherer Absender wird nicht empfohlen**, da diese Methode Ihre Organisation für Spam-, Phishing- und Spoofing-Angriffe anfällig macht.
- Ist dies für Ihr Unternehmen jedoch erforderlich, **empfehlen** wir, **[Regeln zur Nachrichtenübermittlung](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** einzurichten. Unsere Anleitung garantiert die Absenderauthentifizierung (stellt sicher, dass die Absenderdomäne nicht verschleiert wurde). 
    **Hinweis**: Es wird nicht empfohlen, falsche Positivmeldungen mithilfe von Listen sicherer Absender zu verwalten, da Ausnahmen der Spamfilterung Ihre Organisation anfällig für Sicherheitsangriffe machen können. Wenn Ihr(e) Benutzer Nachrichten empfangen, die fälschlicherweise als Spam oder Junk-E-Mail gekennzeichnet sind, sollten Sie diese **[Nachrichten und Dateien an Microsoft melden](https://protection.office.com/reportsubmission)**.
- Sichere Absender in Outlook, Liste zulässiger Absender, oder Liste zulässiger Domänen in Antispamrichtlinien **sollten vermieden werden**, da diese Absender alle Schutzmaßnahmen gegen Spam, Spoofing und Phishing sowie die Absenderauthentifizierung umgehen (SPF, DKIM, DMARC). Diese Methode eignet sich nur für temporäre Tests.
- Die Überprüfung, ob eine bestimmte E-Mail die Antispam-Auswertung umgangen hat, kann durch Überprüfen des Nachrichtenkopfs „X-Forefront-Antispam-Report“ (SFV:SFE, SFV:SKA, SFV:SKN) erfolgen, schauen Sie unter **[Antispam-Nachrichtenkopfzeilen](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Um seine Kunden [standardmäßig zu schützen](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), wendet Microsoft einige Mandantenaußerkraftsetzungen nicht für Schadsoftware und Phishing mit hohem Konfidenzrisiko an. Zu diesen Außerkraftsetzungen gehören: o    Listen zulässiger Absender oder Listen zulässiger Domänen (Antispamrichtlinien) o    Outlook-Richtlinien für sichere Absendender o    Listen zugelassener IP-Adressen (Verbindungsfilterung) 
- Die einzige Außerkraftsetzung, die es Phishing-Nachrichten mit hohem Konfidenzrisiko ermöglicht, die Filterung zu umgehen, sind Exchange-Nachrichtenflussregeln (auch als Transportregeln bezeichnet). Informationen zum Verwenden von Nachrichtenflussregeln zum Umgehen der Filterung finden Sie unter **[Verwenden von Nachrichtenflussregeln zum Festlegen des Spam Confidence Levels (SCL) in Nachrichten](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.