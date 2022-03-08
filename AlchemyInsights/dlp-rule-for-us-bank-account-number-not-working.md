---
title: DLP-Regel für US-Bankkontonummer funktioniert nicht
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b01af4835f44e59395be654b72e86b4e2165a02
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63215709"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-Probleme mit US-Bankkontonummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit US-Bankkontonummern**

Haben Sie Probleme mit **der Verhinderung von Datenverlust (Data Loss Prevention, DLP),** die nicht für Inhalte funktionieren, die eine **US-Bankkontonummer** enthalten, wenn Sie einen vertraulichen DLP-Informationstyp in O365 verwenden? Wenn ja, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für die Suche nach der DLP-Richtlinie enthalten, wenn sie ausgewertet wird.
  
For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 Ziffern

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 bis 17 aufeinander folgende Ziffern.

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Eine DLP-Richtlinie ist zu 75 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Der reguläre Ausdruck Regex_usa_bank_account_number nach Inhalten sucht, die dem Muster entsprechen

  - Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.

    Das folgende Beispiel würde z. B. für die **US-Bankkontonummernrichtlinie** ausgelöst: Überprüfen der 78344011

Weitere Informationen dazu, was erforderlich ist, damit eine **US-Bankkontonummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen nach US-Bankkontonummer suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  