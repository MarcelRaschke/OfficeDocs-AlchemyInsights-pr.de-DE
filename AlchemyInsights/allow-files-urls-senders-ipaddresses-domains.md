---
title: Vorgehensweise Zulassen von Dateien, URLs, Absendern, IP-Adressen und Domänen in Office 365
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "15951"
ms.openlocfilehash: d108296bbb0ac009750abf728873bcbdd4d7c36b
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61949183"
---
# <a name="how-to-allow-files-urls-senders-ip-addresses-and-domains-in-office-365"></a>Vorgehensweise Zulassen von Dateien, URLs, Absendern, IP-Adressen und Domänen in Office 365

**WICHTIG**

Seien Sie vorsichtig, wenn Sie Office 365 Filter umgehen möchten. Microsoft empfiehlt nicht, der LISTE zugelassener IP-Adressen eine IP-Adresse oder einen Adressbereich hinzuzufügen. Es wird auch nicht empfohlen, der Liste der zulässigen Domänen Domänen hinzuzufügen. Weitere Informationen finden Sie unter [Erstellen von Listen sicherer Absender in EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365)

Wenn Sie mit Microsoft-Spam- und Phishing-Bewertungen nicht einverstanden sind, empfehlen wir, Dateien, URLs und Absender in den Mandanten-Zulassungs-/Sperrlisten zuzulassen. Auf diese Weise können wir aus Ihren Übermittlungen lernen und die Filter anpassen, um präzisere Bewertungen zu treffen. Weitere Informationen finden Sie unter [Verwalten Ihrer Berechtigungen in der Mandanten-Zulassungs-/Sperrliste.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-tenant-allows)

1. Wechseln [Sie](https://go.microsoft.com/fwlink/p/?linkid=2077139)im Microsoft 365 Defender Portal zur Seite **"E-Mail &** Übermittlungen für die Zusammenarbeit",  >   wählen Sie die Registerkarte **"Für Analyse übermittelt"** und dann **"Zur Analyse an Microsoft übermitteln"** aus.
2. Wählen Sie im Abschnitt **"Auswählen eines Grunds für die Übermittlung an Microsoft"** die Option **"Sollte nicht blockiert worden sein ( Falsch positiv)** aus.
3. Wählen Sie den Umschalter aus, um die Option **"Nachrichten wie diese zulassen"** zu aktivieren und die Microsoft-Bewertungen außer Kraft zu setzen.
4. Wählen Sie in der Dropdownliste **"Entfernen nach"** aus, wie lange die Option "Zulassen" funktionieren soll. Wenn Sie fertig sind, wählen Sie **Absenden** aus.

Informationen zum Zulassen einer IP-Adresse oder eines Adressbereichs finden Sie unter [Konfigurieren der Standardverbindungsfilterrichtlinie.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy#use-the-microsoft-365-defender-portal-to-modify-the-default-connection-filter-policy)

Fügen Sie der Liste der zulässigen Domänen niemals Ihre eigenen [akzeptierte Domänen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains) oder allgemeine Domänen (z. B. microsoft.com oder office.com) hinzu. Wenn diese Domänen die Spam-Filterung umgehen dürfen, können Angreifer problemlos Nachrichten senden, die diese vertrauenswürdigen Domänen in Ihr Unternehmen spoofen.

Informationen zum Zulassen von Domänen finden Sie unter [Konfigurieren von Spamfilterrichtlinien.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)

Um Absendern das Spoofing und die Anzeige von Spoofingaktivitäten zu ermöglichen, wechseln Sie im Microsoft 365 Defender Portal zu **E-Mail-&**  >  **Zusammenarbeitsrichtlinien &**  >  **Regelbedrohungsrichtlinien**  >  **Mandanten-Zulassungs-/Sperrlisten.** Wählen Sie die Domäne und die sendende Infrastruktur aus, die Domänen spoofen dürfen. Weitere Informationen finden Sie unter "Einblick in die [Spoofintelligenz".](https://docs.microsoft.com/microsoft-365/security/office-365-security/learn-about-spoof-intelligence)
