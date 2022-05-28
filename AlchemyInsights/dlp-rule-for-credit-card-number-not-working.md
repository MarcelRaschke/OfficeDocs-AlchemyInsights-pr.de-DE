---
title: DLP-Regel für Kreditkartennummer funktioniert nicht
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: c0d6f926167a1d62794acaa800c5dab25e81a52b
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65722424"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-Probleme mit Kreditkartennummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit Kreditkartennummern**

Haben Sie Probleme mit Microsoft Purview Data Loss Prevention nicht für Inhalte mit einer **Kreditkartennummer** zu arbeiten, wenn Sie einen vertraulichen DLP-Informationstyp in O365 verwenden? Wenn dies der Fall ist, stellen Sie sicher, dass Ihr Inhalt die erforderlichen Informationen enthält, um die DLP-Richtlinie auszulösen, wenn sie ausgewertet wird. Beispielsweise werden für eine **Kreditkartenrichtlinie** , die mit einem Konfidenzniveau von 85 % konfiguriert ist, Folgendes ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 Ziffern, die formatiert oder unformatiert werden können (dddddddddddd) und den Luhn-Test bestehen müssen.

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Sehr komplexes und robustes Muster, das Karten aller wichtigen Marken weltweit erkennt, einschließlich Visa, MasterCard, Discover Card, JCB, American Express, Geschenkkarten und Diner-Karten.

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, die Luhn-Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Eine DLP-Richtlinie ist zu 85 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.

  - Eine der folgenden Bedingungen trifft zu:

  - Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.

  - Es wird ein Schlüsselwort aus Keyword_cc_name gefunden.

  - Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.

  - Die Prüfsummendurchläufe

    Das folgende Beispiel würde z. B. eine DLP-Kreditkartennummernrichtlinie auslösen:

  - Visum: 4485 3647 3952 7352
  
  - Läuft ab: 02.02.2009

Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen nach Kreditkarte suchen#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  