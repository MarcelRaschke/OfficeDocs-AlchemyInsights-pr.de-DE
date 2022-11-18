---
title: Zulassen von Dateien, URLs, Absendern, IP-Adressen und Domänen in Office 365
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002921"
- "15951"
ms.date: 04/27/2022
ms.openlocfilehash: ede71274053bb623d85286bce2f6cda3f0b85384
ms.sourcegitcommit: b6faebed3da41577a0a16993b065dce49480fa7f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/29/2022
ms.locfileid: "65126608"
---
# <a name="how-to-allow-files-urls-senders-ip-addresses-and-domains-in-office-365"></a>Zulassen von Dateien, URLs, Absendern, IP-Adressen und Domänen in Office 365

**WICHTIG**

Seien Sie vorsichtig, wenn Sie Office 365 Filter umgehen möchten. Microsoft empfiehlt nicht, der IP-Zulassungsliste eine IP-Adresse oder einen Adressbereich hinzuzufügen. Es wird auch nicht empfohlen, der Liste der zulässigen Domänen Domänen hinzuzufügen. Weitere Informationen finden [Sie unter Erstellen von Listen sicherer Absender in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365).

Wenn Sie mit Spam- und Phishingbewertungen von Microsoft nicht einverstanden sind, empfehlen wir, Dass Sie Dateien, URLs und Absender in den Mandanten-Zulassungs-/Sperrlisten zulassen. Auf diese Weise können wir aus Ihren Übermittlungen lernen und die Filter anpassen, um genauere Bewertungen zu treffen. Weitere Informationen finden [Sie unter "Verwalten Ihrer Zulassungen" in der Mandanten-Zulassungs-/Sperrliste](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-tenant-allows).

1. Wechseln Sie im [Microsoft 365 Defender Portal](https://go.microsoft.com/fwlink/p/?linkid=2077139) zur Seite **"Aktionen & ÜbermittlungenSubmissionen** > ", wählen Sie die Registerkarte "**Zur Analyse übermittelt**" und dann "**Zur Analyse an Microsoft übermitteln**" aus.
2. **Wählen Sie im Abschnitt "Grund für die Übermittlung an Microsoft auswählen**" die Option **"Sollte nicht blockiert worden sein " (Falsch positiv)** aus.
3. Wählen Sie den Umschalter aus, um die Option **"Nachrichten wie diese** zulassen" zu aktivieren und die Microsoft-Bewertungen außer Kraft zu setzen.
4. Wählen Sie in der Dropdownliste " **Entfernen nach** " aus, wie lange die Option "Zulassen" funktionieren soll. Wenn Sie fertig sind, wählen Sie **"Absenden**" aus.

Informationen zum Zulassen einer IP-Adresse oder eines Adressbereichs finden [Sie unter Konfigurieren der Standardverbindungsfilterrichtlinie](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy#use-the-microsoft-365-defender-portal-to-modify-the-default-connection-filter-policy).

Fügen Sie der Liste der zulässigen Domänen niemals Ihre eigenen [akzeptierte Domänen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains) oder allgemeine Domänen (z. B. microsoft.com oder office.com) hinzu. Wenn diese Domänen die Spam-Filterung umgehen dürfen, können Angreifer problemlos Nachrichten senden, die diese vertrauenswürdigen Domänen in Ihr Unternehmen spoofen.

Informationen zum Zulassen von Domänen finden [Sie unter Konfigurieren von Spamfilterrichtlinien](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).

Um Absendern das Spoofing zu ermöglichen und Spoofingaktivitäten anzuzeigen, wechseln Sie im Microsoft 365 Defender Portal zu **"E-Mail &** **CollaborationPolicies** >  & **RulesThreat policiesTenant** >  **Allow/Block Lists**". >  Wählen Sie die Domäne und die sendende Infrastruktur aus, die Domänen spoofieren dürfen. Weitere Informationen finden Sie unter [Spoofing Intelligence Insight](https://docs.microsoft.com/microsoft-365/security/office-365-security/learn-about-spoof-intelligence).
