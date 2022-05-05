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
ms.openlocfilehash: 88a5a8732ed30479af952e4affc7ae63df9abac5
ms.sourcegitcommit: 5cdb7885e5ac2787c6616101ee1bc7fb23809427
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2022
ms.locfileid: "65219448"
---
# <a name="required-alchemy-header-h1"></a>Erforderliche Alchemy-Kopfzeile H1

Bewährte Methoden und Richtlinien für die Alchemy-Erstellung:

1. **Schachteln Sie Alchemy nicht Insights in Ordnern:** Dadurch wird die URL-Struktur getrennt.
2. Dateien im **Ordner "AlchemyInsights** " müssen für Leerzeichen Dateinamen in Kleinbuchstaben mit Bindestrichen verwenden. Beispiel: **_how-to-enable-litigation-hold.md_**.
3. Fügen Sie die Bucket-ID und Regel-ID aus dem [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) in das Feld "ms.custom" ein. Beispiel:

```
    ms.custom:
    - 100021
    - 1234
```
4. Festlegen von "ms.date" auf das Veröffentlichungsdatum mithilfe des Formats "mm/dd/yyyy"
5. Verwenden Sie die restlichen Metadaten oben in dieser Datei als Vorlage.
6. Öffnen Sie im [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) die Alchemy-Regelseite, und scrollen Sie nach unten zum **Abschnitt Insights**. Suchen Sie **den Lösungstitel,** und verwenden Sie diesen als Ausgangspunkt für Ihre Titelmetadaten und den H1-Titel. Je nachdem, wie die ursprüngliche Zeichenfolge geschrieben wird, müssen Sie sie möglicherweise bearbeiten, um die Lesbarkeit zu verbessern.

**Hinweis** Alchemy Insights MUSS nur ein einziges H1 an der Spitze haben, oder sie werden in der Produktion brechen.

7. Füllen Sie als Nächstes den Textkörper von Insight mithilfe des Entwurfsmaterials im Abschnitt **"Kundenlösung** " der Seite "Alchemy-Regel" aus.

   - **H2s nicht verwenden** Sie werden nicht gerendert. Verwenden Sie daher **fett formatiert** oder andere Konventionen, um separate Abschnitte zu kennzeichnen.
   - **Html nicht verwenden** Verwenden Sie nur einfachen Markdown.
   - Aufzählungen und nummerierte Listen sind in Ordnung.
   - **Fett** und *kursiv* sind auch in Ordnung zu verwenden.
   - **Verwenden Sie keine internen Links.**
   - Links sollten immer **externe Links zu Webinhalten** oder **Deep-Links zu UI-Elementen** sein. Beispiel: [Diagnose und Behebung von Berechtigungsproblemen bei öffentlichen Ordnern](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) oder [aktiven Benutzern](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
   - Entfernen Sie alle Gebietsschemacodes, oder zeigen Sie ausreichend Zeichenfolgen an. Wenn die URL beispielsweise im Browser `https://docs.microsoft.com/en-us/microsoft-365/commerce/subscriptions/cancel-your-subscription?view=o365-worldwide`wie folgt aussieht, ändern Sie sie in `https://docs.microsoft.com/microsoft-365/commerce/subscriptions/cancel-your-subscription`
   - **Keine Links zu anderen Insight-Artikeln**
   - Bilder werden derzeit nicht offiziell unterstützt, sind aber in der Roadmap enthalten.
   - Lassen Sie am Ende des Artikels eine leere Zeile.

Und das ist wirklich schon ein bisschen zu lang. Bewährte Methode sind etwa 400 Zeichen ---------------------------------

Sobald Ihre Inhalte bereit sind, senden Sie eine Pull-Anforderung an den Live Branch. Wechseln Sie dann zum [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das URL-Feld ein.
