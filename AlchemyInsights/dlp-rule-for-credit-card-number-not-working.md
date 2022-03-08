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
ms.openlocfilehash: ba4e70ee0ef5b548256e4fb3a8d4e57fed82d8de
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63277901"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-Probleme mit Kreditkartennummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit Kreditkartennummern**

Haben Sie Probleme mit **der Verhinderung von Datenverlust (Data Loss Prevention, DLP),** die nicht für Inhalte funktionieren, die eine **Kreditkartennummer** enthalten, wenn Sie einen vertraulichen DLP-Informationstyp in O365 verwenden? Wenn ja, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn sie ausgewertet wird. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddd) formatiert werden können und den Luhn-Test bestehen müssen.

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Sehr komplexes und robustes Muster, das Karten von allen wichtigen Marken weltweit erkennt, einschließlich Visa, MasterCard, Discover Card, JCB, American Express, Beschenkungskarten und Dinerkarten.

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, die Luhn-Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Eine DLP-Richtlinie ist zu 85 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.

  - Eine der folgenden Bedingungen trifft zu:

  - Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.

  - Ein Schlüsselwort aus Keyword_cc_name gefunden wird

  - Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.

  - Die Prüfsumme besteht

    Das folgende Beispiel würde beispielsweise für eine DLP-Kreditkartennummernrichtlinie ausgelöst:

  - Visa: 4485 3647 3952 7352
  
  - Läuft ab: 2/2009

Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen nach Kreditkarte suchen#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  