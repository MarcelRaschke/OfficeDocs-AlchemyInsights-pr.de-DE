---
title: DLP benötigt möglicherweise einen benutzerdefinierten Typ
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 75a61e0ef35b67ad2fb635d95d9eb630a75cbd51
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63226941"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP benötigt möglicherweise einen benutzerdefinierten Typ

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp**

Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen. In einigen Szenarien müssen Sie möglicherweise Einen eigenen benutzerdefinierten vertraulichen Informationstyp erstellen, um die Daten Ihrer Organisation zu schützen. Weitere Informationen finden Sie unter [Informationen zu Typen vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) und [Entitätsdefinitionen für Typen vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Weitere Informationen zum Erstellen benutzerdefinierter Typen und Richtlinien für vertrauliche Informationen finden Sie unter: 

**Anpassen eines integrierten, vertraulichen Informationstyps**

Wenn ein integrierter vertraulicher Informationstyp Mit nur wenigen Optimierungen Ihren Anforderungen entspricht, lesen Sie " [Anpassen eines integrierten vertraulichen Informationstyps"](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Sie können z. B. Schlüsselwörter hinzufügen oder entfernen oder unterstützende Nachweise wie z. B. ein Datum oder eine Adresse hinzufügen oder entfernen.

**Erstellen eines benutzerdefinierten vertraulichen Informationstyps**

Wenn Sie jedoch einen anderen Typ vertraulicher Informationen vollständig identifizieren und schützen müssen, können Sie einen benutzerdefinierten vertraulichen Informationstyp im Microsoft 365 Compliance Center erstellen. Weitere Informationen finden Sie unter [Erste Schritte mit benutzerdefinierten Typen vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**

Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie einen benutzerdefinierten Typ vertraulicher Informationen in Security & Compliance Center PowerShell erstellen. Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten vertraulichen Informationstyps mithilfe von PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Informationen zum testen der Richtlinie im Testmodus finden Sie unter [Implementieren der Richtlinie im Testmodus](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) und [Erstellen, Testen und Optimieren einer DLP-Richtlinie](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy). 