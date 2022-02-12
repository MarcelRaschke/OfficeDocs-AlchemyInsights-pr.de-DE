---
title: DLP-Regel für SSN funktioniert nicht
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 6b96813293684ae1fa3eaaa6b28ececfef6305ac
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62759843"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-Probleme mit Sozialversicherungsnummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit SSNs**

Haben Sie Probleme mit **der Verhinderung von Datenverlust (Data Loss Prevention, DLP),** die nicht für Inhalte funktionieren, die eine **Sozialversicherungsnummer (SSN)** enthalten, wenn Sie einen vertraulichen Informationstyp in Microsoft 365 verwenden? Wenn ja, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für die DLP-Richtlinie enthalten. 
  
For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 Ziffern, die in einem formatierten oder unformatierten Muster sein können

- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier Funktionen suchen nach SSNs in vier verschiedenen Mustern:

  - Func_ssn findet SSNs mit vor 2011 starker Formatierung, die mit Strichen oder Leerzeichen formatiert sind (ddd-dd-dddd OR ddd dddd)

  - Func_unformatted_ssn findet SSNs mit starker Formatierung vor 2011, die als neun aufeinander folgende Ziffern unformatiert sind (ddddddddd).

  - Func_randomized_formatted_ssn sucht nach 2011 SSNs, die mit Gedankenstrichen oder Leerzeichen formatiert sind (ddd-dd-dddd OR ddd dd dddd)

  - Func_randomized_unformatted_ssn sucht nach 2011 SSNs, die als neun aufeinander folgende Ziffern unformatiert sind (dddddddddd)

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Eine DLP-Richtlinie ist zu 85 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Die [Funktion Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) nach Inhalten sucht, die dem Muster entsprechen.

  - Ein Schlüsselwort aus [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) wurde gefunden. Beispiele für Schlüsselwörter sind:  *Sozialversicherung, Sozialversicherung#, Soc Sec , SSN*  . Das folgende Beispiel würde beispielsweise für die DLP-SSN-Richtlinie ausgelöst: **SSN: 489-36-8350**
  
Weitere Informationen dazu, was erforderlich ist, damit SSNs für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen nach SSNs suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  