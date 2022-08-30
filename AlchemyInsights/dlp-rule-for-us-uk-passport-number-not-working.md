---
title: DLP-Regel für US/UK Passport Number funktioniert nicht
ms.author: chrfox
author: chrfox
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3200001"
- "1319"
ms.date: 04/21/2020
ms.openlocfilehash: f3082fa71555b77d4aba36cf8e33775ae05ea76f
ms.sourcegitcommit: de048ec631aaa5712637a76a2d1e2c2d18fac720
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2022
ms.locfileid: "67461911"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme mit DLP – US/UK-Reisepassnummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit US/UK-Reisepassnummern**

Haben Sie Probleme mit Microsoft Purview Data Loss Prevention bei der Verwendung eines vertraulichen DLP-Informationstyps in O365 nicht für Inhalte mit einer **US/UK-Reisepassnummer** arbeiten? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dazu enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.
  
For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Neun Ziffern

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Neun aufeinander folgende Ziffern

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Eine DLP-Richtlinie ist zu 75 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Die Funktion Func_usa_uk_passport findet Inhalte, die dem Muster entsprechen.

  - Ein Schlüsselwort aus Keyword_passport wurde gefunden.

    Das folgende Beispiel würde z. B. für die **Us/UK Passport Number** Policy ausgelöst: U.S. Passport number 123456789

Weitere Informationen dazu, was erforderlich ist, damit eine US/UK Passport Number für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen nach US/UK Passport Number suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  