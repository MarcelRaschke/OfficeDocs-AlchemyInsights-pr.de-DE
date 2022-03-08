---
title: identisch mit h1-Überschrift
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- bucket id
- rule id
ms.date: 01/01/2022
ms.openlocfilehash: 235c9ddd3d35f949a16a77fe0d4ef43adabafa9a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63113500"
---
# <a name="required-alchemy-header-h1"></a>Erforderlicher Alemy-Header H1

Bewährte Methoden und Richtlinien für die Alchemy-Erstellung:

1. **Schachteln Sie Alemy Insights nicht in Ordnern:** Dadurch wird die URL-Struktur beschädigt.
2. Dateien im Ordner **"AlchemyInsights** " müssen Dateinamen in Kleinbuchstaben mit Bindestrichen für Leerzeichen verwenden. Beispiel: **_how-to-enable-litigation-hold.md_**.
3. Fügen Sie die Bucket-ID und die Regel-ID aus dem [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) in das Feld "ms.custom" ein. Beispiel:

```
    ms.custom:
    - 100021
    - 1234
```
4. Festlegen des Datums "ms.date" auf das Veröffentlichungsdatum im Format mm/dd/jjjj
5. Verwenden Sie die restlichen Metadaten oben in dieser Datei als Vorlage.
6. Öffnen Sie im [Portal "Alchemy Partner"](https://alchemyportal.azurewebsites.net) die Seite "Alchemy-Regel", und scrollen Sie nach unten zum Abschnitt **"Einblicke** ". Suchen Sie den **Lösungstitel,** und verwenden Sie diesen als Ausgangspunkt für Ihre Titelmetadaten und den H1-Titel. Je nachdem, wie die ursprüngliche Zeichenfolge geschrieben wird, müssen Sie sie möglicherweise zur besseren Lesbarkeit bearbeiten.

**Hinweis** Alemy Insights DARF nur einen einzelnen H1 oben haben, sonst werden sie in der Produktion beschädigt.

7. Füllen Sie als Nächstes den Textkörper "Insight" mithilfe des Entwurfsmaterials im Abschnitt **"Kundenlösung** " der Seite "Alchemy-Regel" aus.

   - **Verwenden Sie keine H2s** Sie werden nicht gerendert. Verwenden Sie daher **fett oder** andere Konventionen, um separate Abschnitte zu kennzeichnen.
   - **Verwenden Sie keinen HTML-Code** Verwenden Sie nur einfaches Markdown.
   - Aufzählungen und nummerierte Listen sind in Ordnung.
   - **Fett** und *kursiv* sind ebenfalls gut zu verwenden.
   - **Verwenden Sie keine internen Links.**
   - Links sollten immer **entweder externe Links zu Webinhalten** oder **Deep-Links zu UI-Elementen** sein. Beispiel: [So diagnostizieren und beheben Sie Berechtigungsprobleme für öffentliche Ordner](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) oder [aktive Benutzer](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
   - Entfernen Sie alle Gebietsschemacodes, oder zeigen Sie ausreichend Zeichenfolgen an. Wenn die URL z. B. im Browser https://docs.microsoft.com/en-us/microsoft-365/commerce/subscriptions/cancel-your-subscription?view=o365-worldwidewie folgt aussieht, ändern Sie sie in https://docs.microsoft.com/microsoft-365/commerce/subscriptions/cancel-your-subscription
   - **Keinen Link zu anderen Insight-Artikeln**
   - Bilder werden derzeit nicht offiziell unterstützt, aber sie sind in der Roadmap enthalten.
   - Lassen Sie am Ende des Artikels eine leere Zeile.

Und dies ist eigentlich schon ein wenig zu lang. Bewährte Methode ist etwa 400 Zeichen ---------------------------------

Sobald Ihre Inhalte bereit sind, senden Sie eine Pull-Anforderung an die Live-Verzweigung. Wechseln Sie dann zum [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das FELD "URL" ein.
