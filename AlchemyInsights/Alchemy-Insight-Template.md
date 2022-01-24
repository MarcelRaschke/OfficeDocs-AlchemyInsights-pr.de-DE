---
title: (identisch mit h1-Überschrift)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- (bucket id)
- (rule id)
ms.date: (publish date)
ms.openlocfilehash: 3ddf7f6b6e0e4c1239303f7cacc0f0e596f9f0e0
ms.sourcegitcommit: 5dcbecdebbf5042db0c86a12149ddd537d766c91
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2022
ms.locfileid: "62185204"
---
# <a name="required-alchemy-header-h1"></a>"Erforderlicher Alchimy-Header H1"

Bewährte Methoden und Richtlinien für die Alchemy-Erstellung:

1. **Schachteln Sie Alchemy-Insights nicht in Ordnern:** Dadurch wird die URL-Struktur beschädigt.
1. Dateien im Ordner **"AlchemyInsights"** müssen Dateinamen mit Bindestrichen für Leerzeichen in Kleinbuchstaben schreiben. Beispiel: **_how-to-enable-litigation-hold.md_**.
1. Fügen Sie die Bucket-ID und die Regel-ID aus dem [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) in das Feld "ms.custom" ein. Zum Beispiel:

```
    ms.custom:
    - 100021
    - 1234
```

1. Verwenden Sie die restlichen Metadaten oben in dieser Datei als Vorlage.
1. Öffnen Sie im [Portal "Alchemy Partner"](https://alchemyportal.azurewebsites.net) die Seite "Alchemy-Regel", und scrollen Sie nach unten zum **Abschnitt Insights.** Suchen Sie den **Lösungstitel,** und verwenden Sie diesen als Ausgangspunkt für Ihre Titelmetadaten und den H1-Titel. Je nachdem, wie die ursprüngliche Zeichenfolge geschrieben wird, müssen Sie sie möglicherweise zur besseren Lesbarkeit bearbeiten.

**Hinweis** Alchemy Insights DARF nur einen einzelnen H1 oben haben, sonst werden sie in der Produktion beschädigt.

1. Füllen Sie als Nächstes den Textkörper "Insight" mithilfe des Entwurfsmaterials im Abschnitt **"Kundenlösung"** der Seite "Alchemy-Regel" aus.

   - **Verwenden Sie keine H2s** Sie werden nicht gerendert. Verwenden Sie daher **fett oder** andere Konventionen, um separate Abschnitte zu kennzeichnen.
   - **Verwenden Sie keinen HTML-Code** Verwenden Sie nur einfaches Markdown.
   - Aufzählungen und nummerierte Listen sind in Ordnung.
   - **Fett** und *kursiv* sind ebenfalls gut zu verwenden.
   - **Verwenden Sie keine internen Links.**
   - Links sollten immer **entweder externe Links zu Webinhalten** oder **Deep-Links zu UI-Elementen** sein. Beispiel: [So diagnostizieren und beheben](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) Sie Berechtigungsprobleme für öffentliche Ordner oder [aktive Benutzer.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
   - **Keinen Link zu anderen Insight-Artikeln**
   - Bilder werden derzeit nicht offiziell unterstützt, aber sie sind in der Roadmap enthalten.
   - Lassen Sie am Ende des Artikels eine leere Zeile.

Und dies ist eigentlich schon ein wenig zu lang. Bewährte Methode ist etwa 400 Zeichen ---------------------------------

Sobald Ihre Inhalte bereit sind, senden Sie eine Pull-Anforderung an die Live-Verzweigung. Wechseln Sie dann zum [Alchemy Partner-Portal,](https://alchemyportal.azurewebsites.net) und geben Sie den Dateinamen in das FELD "URL" ein.
