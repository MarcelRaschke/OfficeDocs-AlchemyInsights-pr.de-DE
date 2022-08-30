---
title: DLP-Regel für US-Bankkontonummer funktioniert nicht
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
- "1287"
ms.date: 04/21/2020
ms.openlocfilehash: 7acc1703f089fd632e7a7d3dec5ae0fd7cf6d1ee
ms.sourcegitcommit: de048ec631aaa5712637a76a2d1e2c2d18fac720
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2022
ms.locfileid: "67461822"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-Probleme mit US-Bankkontonummern

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP-Probleme mit US-Bankkontonummern**

Haben Sie Probleme mit Microsoft Purview Data Loss Prevention nicht für Inhalte mit einer **US-Bankkontonummer** arbeiten, wenn Sie einen vertraulichen DLP-Informationstyp in O365 verwenden? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dazu enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.
  
Beispielsweise werden für eine **Richtlinie für die US-Bankkontonummer** , die mit einem Konfidenzniveau von 85 % konfiguriert ist, Folgendes ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 Ziffern

- **[Muster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 aufeinander folgende Ziffern.

- **[Prüfsumme:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Eine DLP-Richtlinie ist zu 75 % sicher, dass diese Art vertraulicher Informationen erkannt wird, wenn innerhalb einer Näherung von 300 Zeichen:

  - Der reguläre Ausdruck Regex_usa_bank_account_number findet Inhalt, der dem Muster entspricht.

  - Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.

    Das folgende Beispiel würde z. B. die Richtlinie für die **US-Bankkontonummer** auslösen: Konto 78344011

Weitere Informationen dazu, was erforderlich ist, damit eine **US-Bankkontonummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [Wonach die Typen vertraulicher Informationen für die US-Bankkontonummer suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen dazu, was für andere Typen erforderlich ist: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  