---
title: Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 27653b0e535a4dc237a6a87efe1bafe1d30ded0d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63306149"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?

- **Es wird nicht empfohlen, Listen sicherer Absender zu verwenden**, da diese Ihre Organisation für Spam-, Phishing- und Spoofingangriffe öffnen.
- Wenn Sie in Ihrem Unternehmen jedoch die Filterung nach bestimmten Nachrichten umgehen müssen, **empfehlen** wir die Verwendung von **[Nachrichtenflussregeln](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365#recommended-use-mail-flow-rules)** (auch als Transportregeln bezeichnet). Unsere Anleitung garantiert die Absenderauthentifizierung (stellt sicher, dass die Absenderdomäne nicht verschleiert wurde).

    **Hinweis**: Es wird nicht empfohlen, falsche Positivmeldungen mithilfe von Listen sicherer Absender zu verwalten, da Ausnahmen der Spamfilterung Ihre Organisation anfällig für Sicherheitsangriffe machen können. Wenn Ihr(e) Benutzer Nachrichten empfangen, die fälschlicherweise als Spam oder Junk-E-Mail gekennzeichnet sind, sollten Sie diese **[Nachrichten und Dateien an Microsoft melden](https://protection.office.com/reportsubmission)**.

- Sichere Absender in Outlook, Listen zulässiger Absender oder zulässiger Domänen in Anti-Spam-Richtlinien **sollten vermieden werden**, da diese Absender alle Schutzmaßnahmen zu Spam, Spoofing und Phishing sowie die Absenderauthentifizierung umgehen (SPF, DKIM, DMARC). Diese Methoden werden am besten nur für temporäre Tests verwendet.
- Sie können überprüfen, ob eine Antispam-Auswertung für Nachrichten erfolgt, indem Sie den Nachrichtenkopf **X-Forefront-Antispam-Report** (`SFV:SFE`, `SFV:SKA`, `SFV:SKN`) überprüfen. Weitere Informationen finden Sie unter [Antispam-Nachrichtenkopfzeilen](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers).
- Um seine Kunden [standardmäßig zu schützen](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), lässt Microsoft einige Außerkraftsetzungen für E-Mails mit hoher Schadsoftware- oder Phishingwahrscheinlichkeit nicht zu. Diese Außerkraftsetzungen enthalten:
  - Listen zulässiger Absender oder Listen zulässiger Domänen (Antispamrichtlinien).
  - Outlook Safe Senders (Sichere Absender in Outlook).
  - Liste zugelassener IP-Adressen (Verbindungsfilterrichtlinien).
- Die einzige Außerkraftsetzung, die es E-Mails mit hoher Phishingwahrscheinlichkeit ermöglicht, die Filterung zu umgehen, sind Nachrichtenflussregeln. Informationen zum Verwenden von Nachrichtenflussregeln zum Umgehen der Filterung finden Sie unter [Verwenden von Nachrichtenflussregeln zum Festlegen des Spam Confidence Levels (SCL) in Nachrichten](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/use-rules-to-set-scl).
