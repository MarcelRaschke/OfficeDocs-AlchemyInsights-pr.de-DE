---
title: eDiscovery-Export bleibt hängen oder erzeugt Zero-Byte-Datei
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000661"
- "16357"
ms.date: 01/21/2022
ms.openlocfilehash: 16b3ebea24e602941d953279597de5c813cf51d6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66435424"
---
# <a name="ediscovery-export-stuck-or-produces-zero-byte-file"></a>eDiscovery-Export bleibt hängen oder erzeugt Zero-Byte-Datei

Wenn ihr eDiscovery-Export hängen bleibt oder während des Exports eine Zero-Byte-Datei erzeugt, versuchen Sie Folgendes:

1. Verwenden Sie einen anderen Client zum Herunterladen.
2. Entfernen Sie Suchvorgänge, die nicht mehr erforderlich sind, indem Sie das Cmdlet [Remove-ComplianceSearch](https://docs.microsoft.com/powershell/module/exchange/remove-compliancesearch?view=exchange-ps&preserve-view=true) ausführen.
3. Stellen Sie sicher, dass Sie auf ein lokales Laufwerk herunterladen.
4. Stellen Sie sicher, dass der Virenscanner nicht ausgeführt wird.
5. Stellen Sie sicher, dass kein anderer Export in denselben Ordner oder einen übergeordneten Ordner heruntergeladen wird.
6. Wenn die vorherigen Schritte nicht funktionieren, deaktivieren Sie zipping und Deduplizierung.
7. Wenn Schritt 6 funktioniert, liegt das Problem an einem lokalen Virenscanner oder einem Datenträgerproblem.

**Hinweis**: Beim Anzeigen der datei trace.log (befindet sich in dem Ordner, in dem Sie den Inhalt exportieren), sehen Sie möglicherweise einen Fehler in der Datei ähnlich dem folgenden: "Hit tolerable error, will retry: The process cannot access the file 'ExportData.db' because it is being used by another process."

Weitere Schritte zur Problembehandlung für eDiscovery-Exporte finden [Sie unter Beheben häufiger eDiscovery-Probleme: Erträglicher Fehler](https://docs.microsoft.com/office365/troubleshoot/ediscovery/resolve-ediscovery-issues#error-hit-tolerable-error-will-retry-the-process-cannot-access-the-file-exportdatadb-because-it-is-being-used-by-another-process).
