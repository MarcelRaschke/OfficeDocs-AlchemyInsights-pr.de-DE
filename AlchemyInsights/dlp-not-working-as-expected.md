---
title: DLP funktioniert nicht wie erwartet
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079701"
---
# <a name="dlp-not-working-as-expected"></a>DLP funktioniert nicht wie erwartet

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

 **Einrichten von DLP**

Haben Sie Probleme mit **der Verhinderung von Datenverlust (Data Loss Prevention, DLP)** in Office 365 nicht wie erwartet funktionieren? Wenn ja, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die **DLP-Richtlinie** sucht, wenn sie ausgewertet wird.
  
Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen. Verwenden Sie die [hier aufgeführten](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)Informationen, um DLP-Richtlinien einzurichten.
  
 **Wonach DLP-Richtlinien suchen**
  
Bei Verwendung der **integrierten Typen vertraulicher Informationen** im Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.
  
- **Integrierte Typen vertraulicher Informationen**

    Informationen zu den integrierten vertraulichen Typen und zu den Suchzwecken einer DLP-Richtlinie beim Erkennen des vertraulichen Typs finden Sie unter: [Wonach die Typen vertraulicher Informationen suchen.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Benutzerdefinierte Typen vertraulicher Informationen**

    Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten vertraulichen Informationstyps.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testen einer DLP-Richtlinie**

Um Ihre Daten mit einem integrierten oder benutzerdefinierten vertraulichen Informationstyp zu testen, verwenden Sie die Option **"Testtyp"** unter **"Klassifizierungen**  >  **vertraulicher Informationstypen".** Weitere Informationen finden Sie unter [Testen benutzerdefinierter Typen vertraulicher Informationen.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Berichte**
  
- Erhalten Sie einblicke in vertrauliche Daten mit [DLP-Berichten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Sehen Sie sich spezifische Details des Ereignisses mit einem [Vorfallbericht an.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
