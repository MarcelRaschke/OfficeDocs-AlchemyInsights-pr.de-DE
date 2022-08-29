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
ms.date: 08/24/2022
ms.openlocfilehash: bd5fa5c5b362f420a64b60d6ca6670ecc4ecb144
ms.sourcegitcommit: 26ebd27a7a98a0730483d243bb196cb214330c08
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/24/2022
ms.locfileid: "67426342"
---
# <a name="dlp-not-working-as-expected"></a>DLP funktioniert nicht wie erwartet

Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen. Informationen zum Einrichten von DLP-Richtlinien finden [Sie unter Erstellen einer DLP-Richtlinie anhand einer Vorlage](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).

**Wonach DLP-Richtlinien suchen**

Bei Verwendung der integrierten Typen vertraulicher Informationen in den Security and Compliance Centern suchen DLP-Richtlinien nach bestimmten Mustern und Elementen.

- **Integrierte Typen vertraulicher Informationen**

    Informationen zu den integrierten vertraulichen Typen und dazu, wonach eine DLP-Richtlinie beim Erkennen der vertraulichen Typen sucht, finden Sie unter [Entitätsdefinitionen für vertrauliche Informationstypen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Benutzerdefinierte Typen vertraulicher Informationen**

    Wenn Sie benutzerdefinierte Typen vertraulicher Informationen erstellen, lesen [Sie "Erstellen von benutzerdefinierten Typen vertraulicher Informationen" im Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testen einer DLP-Richtlinie**

Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten vertraulichen Informationstyp testen möchten, verwenden Sie die Option **"Testtyp** " unter **"Klassifizierungen** > **vertraulicher Informationstypen**". Weitere Informationen finden Sie unter ["Testen eines vertraulichen Informationstyps"](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#test-a-sensitive-information-type).

**Berichte**

- Erhalten Sie Einblicke in vertrauliche Daten mit [DLP-Berichten](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports).

- Zeigen Sie Details des Ereignisses mit einem [Vorfallbericht an](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).