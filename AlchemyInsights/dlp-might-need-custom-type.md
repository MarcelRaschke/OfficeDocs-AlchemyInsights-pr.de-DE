---
title: DLP benötigt möglicherweise einen benutzerdefinierten Typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030793"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP benötigt möglicherweise einen benutzerdefinierten Typ

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp**

Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen. In einigen Szenarien müssen Sie möglicherweise Einen eigenen **benutzerdefinierten** vertraulichen Informationstyp erstellen, um die Daten Ihrer Organisation zu schützen.

Beispielsweise muss Ihre Organisation möglicherweise Mitarbeiter-IDs oder andere Daten in einem für Ihre Organisation spezifischen Format identifizieren und schützen. Wenn ja, finden Sie weitere Informationen in den folgenden Artikeln.
  
 **Anpassen eines integrierten, vertraulichen Informationstyps**
  
Wenn ein integrierter vertraulicher Informationstyp Ihren Anforderungen mit nur wenigen Optimierungen entspricht, können Sie [einen integrierten vertraulichen Informationstyp anpassen.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Sie können z. B. Schlüsselwörter hinzufügen oder entfernen oder unterstützende Nachweise wie z. B. ein Datum oder eine Adresse hinzufügen oder entfernen.
  
 **Erstellen eines benutzerdefinierten vertraulichen Informationstyps**
  
Wenn Sie jedoch einen anderen Typ vertraulicher Informationen vollständig identifizieren und schützen müssen, können Sie auf der Benutzeroberfläche des Security & Compliance Centers [einen benutzerdefinierten Typ vertraulicher Informationen erstellen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)
  
**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**

Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie [einen benutzerdefinierten vertraulichen Informationstyp in Security & Compliance Center PowerShell erstellen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden.
