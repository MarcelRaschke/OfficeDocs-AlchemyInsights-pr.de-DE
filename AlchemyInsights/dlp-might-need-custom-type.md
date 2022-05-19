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
ms.openlocfilehash: 9bbd8a86f4666b66ee99465602e1aba94255c64b
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65593408"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP benötigt möglicherweise einen benutzerdefinierten Typ

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp**

Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen. In einigen Szenarien müssen Sie möglicherweise Einen eigenen benutzerdefinierten vertraulichen Informationstyp erstellen, um die Daten Ihrer Organisation zu schützen. Weitere Informationen finden Sie unter [Informationen zu Typen vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) und [Entitätsdefinitionen für vertrauliche Informationstypen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Weitere Informationen zum Erstellen benutzerdefinierter vertraulicher Informationstypen und Richtlinien finden Sie unter: 

**Anpassen eines integrierten, vertraulichen Informationstyps**

Wenn ein integrierter vertraulicher Informationstyp Ihre Anforderungen mit nur wenigen Optimierungen erfüllen würde, lesen [Sie "Anpassen eines integrierten vertraulichen Informationstyps](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)". Sie können z. B. Schlüsselwörter hinzufügen oder entfernen oder unterstützende Nachweise wie ein Datum oder eine Adresse hinzufügen oder entfernen.

**Erstellen eines benutzerdefinierten vertraulichen Informationstyps**

Wenn Sie jedoch einen anderen Typ vertraulicher Informationen vollständig identifizieren und schützen müssen, können Sie einen benutzerdefinierten vertraulichen Informationstyp in der Microsoft Purview-Complianceportal erstellen. Weitere Informationen finden Sie [unter Erste Schritte mit benutzerdefinierten typen vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**

Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie im Security & Compliance Center PowerShell einen benutzerdefinierten vertraulichen Informationstyp erstellen. Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten vertraulichen Informationstyps mithilfe von PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Wenn Sie Ihre Richtlinie zuerst im Testmodus testen möchten, lesen [Sie "Richtlinie im Testmodus implementieren](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) " und ["Erstellen, Testen und Optimieren einer DLP-Richtlinie](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy)". 