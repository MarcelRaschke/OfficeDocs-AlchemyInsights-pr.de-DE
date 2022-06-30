---
title: DLP-Regel für SSN funktioniert nicht
ms.author: deniseb
author: denisebmsft
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3200001"
- "1242"
ms.date: 04/21/2020
ms.openlocfilehash: dbac6d3e081e56435c1dffd6f8b75b2a7c715c2e
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66509171"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-Probleme mit Sozialversicherungsnummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit SSNs**

Haben Sie Probleme mit Microsoft Purview Data Loss Prevention bei der Verwendung eines vertraulichen Informationstyps in Microsoft 365 nicht für Inhalte mit einer **Sozialversicherungsnummer (Social Security Number, SSN)** zu arbeiten? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für das, was die DLP-Richtlinie sucht, enthalten. 
  
Für eine SSN-Richtlinie, die mit einem Konfidenzniveau von 85 % konfiguriert ist, werden beispielsweise Folgendes ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 Ziffern, die in einem formatierten oder unformatierten Muster vorliegen können

- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier Funktionen suchen nach SSNs in vier verschiedenen Mustern:

  - Func_ssn findet SSNs mit starker Formatierung vor 2011, die mit Strichen oder Leerzeichen formatiert sind (ddd-dd-dddd OR ddd dd dd ddd)

  - Func_unformatted_ssn findet SSNs mit starker Formatierung vor 2011, die als neun aufeinander folgende Ziffern unformatiert sind (dddddddddd)

  - Func_randomized_formatted_ssn findet SSNs nach 2011, die mit Bindestrichen oder Leerzeichen formatiert sind (ddd-dd-dddd OR ddd dd dd ddd)

  - Func_randomized_unformatted_ssn findet SSNs nach 2011, die als neun aufeinander folgende Ziffern unformatiert sind (ddddddddddd)

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Eine DLP-Richtlinie ist zu 85 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Die [Funktion Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) findet Inhalt, der dem Muster entspricht.

  - Ein Schlüsselwort aus [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) wurde gefunden. Beispiele für Schlüsselwörter sind:  *Sozialversicherung, Sozialversicherung#, Soc Sec , SSN*  . Das folgende Beispiel würde beispielsweise für die DLP-SSN-Richtlinie ausgelöst **: SSN: 489-36-8350**
  
Weitere Informationen dazu, was erforderlich ist, damit SSNs für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen nach SSNs suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  