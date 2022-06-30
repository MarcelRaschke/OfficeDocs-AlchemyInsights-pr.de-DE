---
title: DLP funktioniert nicht wie erwartet
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
- "1241"
ms.date: 04/21/2020
ms.openlocfilehash: 65ee79544848036f00fa5b9720fb4cf23c6bd830
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66509154"
---
# <a name="dlp-not-working-as-expected"></a>DLP funktioniert nicht wie erwartet

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

 **Einrichten von DLP**

Haben Sie Probleme mit Microsoft Purview Data Loss Prevention in Office 365 nicht wie erwartet? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre DLP-Richtlinie ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die DLP-Richtlinie sucht, wenn sie ausgewertet wird.
  
Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen. Verwenden Sie die [hier](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) aufgeführten Informationen, um DLP-Richtlinien einzurichten.
  
 **Wonach DLP-Richtlinien suchen**
  
Bei Verwendung der **integrierten Typen vertraulicher Informationen** in den Security and Compliance Centern suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.
  
- **Integrierte Typen vertraulicher Informationen**

    Informationen zu den integrierten Typen vertraulicher Informationen und dazu, wonach eine DLP-Richtlinie beim Erkennen des Typs "Vertraulich" sucht, finden Sie unter: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Benutzerdefinierte Typen vertraulicher Informationen**

    Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten vertraulichen Informationstyps](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testen einer DLP-Richtlinie**

Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten vertraulichen Informationstyp testen möchten, verwenden Sie die Option **"Testtyp** " unter **"Klassifizierungen** > **vertraulicher Informationstypen**". Weitere Informationen finden Sie unter ["Testen benutzerdefinierter vertraulicher Informationstypen"](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Berichte**
  
- Erhalten Sie Einblicke in vertrauliche Daten mit [DLP-Berichten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Sehen Sie sich spezifische Details des Ereignisses mit einem [Vorfallbericht an](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
