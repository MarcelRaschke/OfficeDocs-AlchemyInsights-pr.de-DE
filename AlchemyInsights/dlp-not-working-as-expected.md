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
ms.openlocfilehash: 63c093f184ffe842443f7df3eb1f2f89815ebfa2
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62710917"
---
# <a name="dlp-not-working-as-expected"></a>DLP funktioniert nicht wie erwartet

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

 **Einrichten von DLP**

Haben Sie Probleme mit **der Verhinderung von Datenverlust (Data Loss Prevention, DLP)** in Office 365 nicht wie erwartet funktionieren? Wenn ja, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die **DLP-Richtlinie** sucht, wenn sie ausgewertet wird.
  
Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen. Verwenden Sie die [hier](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) aufgeführten Informationen, um DLP-Richtlinien einzurichten.
  
 **Wonach DLP-Richtlinien suchen**
  
Bei Verwendung der **integrierten Typen vertraulicher Informationen** im Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.
  
- **Integrierte Typen vertraulicher Informationen**

    Informationen zu den integrierten vertraulichen Typen und zu den Suchzwecken einer DLP-Richtlinie beim Erkennen des vertraulichen Typs finden Sie unter: [Wonach die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Benutzerdefinierte Typen vertraulicher Informationen**

    Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten vertraulichen Informationstyps](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testen einer DLP-Richtlinie**

Um Ihre Daten mit einem integrierten oder benutzerdefinierten vertraulichen Informationstyp zu testen, verwenden Sie die Option **"Testtyp** " unter den Informationstypen **"ClassificationsSensitive** > **"**. Weitere Informationen finden Sie unter [Testen benutzerdefinierter Typen vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Berichte**
  
- Erhalten Sie einblicke in vertrauliche Daten mit [DLP-Berichten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Sehen Sie sich bestimmte Details des Ereignisses mit einem [Vorfallbericht an](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
