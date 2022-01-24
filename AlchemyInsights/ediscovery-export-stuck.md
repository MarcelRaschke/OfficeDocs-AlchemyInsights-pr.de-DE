---
title: eDiscovery-Export bleibt hängen oder erzeugt Null-Byte-Datei
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "16357"
ms.date: 01/21/2022
ms.openlocfilehash: 5296641a17f4db5d5b6261b213a553c0bd0e799c
ms.sourcegitcommit: 5dcbecdebbf5042db0c86a12149ddd537d766c91
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2022
ms.locfileid: "62185345"
---
# <a name="ediscovery-export-stuck-or-produces-zero-byte-file"></a>eDiscovery-Export bleibt hängen oder erzeugt Null-Byte-Datei

Wenn Ihr eDiscovery-Export während des Exports hängen bleibt oder eine Null-Byte-Datei erzeugt, versuchen Sie Folgendes:

1. Verwenden Sie einen anderen Client zum Herunterladen.
2. Entfernen Sie Suchen, die nicht mehr benötigt werden, indem Sie das Cmdlet [Remove-ComplianceSearch](https://docs.microsoft.com/powershell/module/exchange/remove-compliancesearch?view=exchange-ps&preserve-view=true)ausführen.
3. Stellen Sie sicher, dass Sie auf ein lokales Laufwerk herunterladen.
4. Stellen Sie sicher, dass der Virenscanner nicht ausgeführt wird.
5. Stellen Sie sicher, dass kein anderer Export in denselben Ordner oder einen übergeordneten Ordner heruntergeladen wird.
6. Wenn die vorherigen Schritte nicht funktionieren, deaktivieren Sie Zipping und Deduplizierung.
7. Wenn Schritt 6 funktioniert, liegt das Problem an einem lokalen Virenscanner oder einem Datenträgerproblem.

**Hinweis:** Beim Anzeigen der Datei "trace.log" (befindet sich in dem Ordner, in den Sie den Inhalt exportieren), wird möglicherweise ein Fehler in der Datei angezeigt, der dem folgenden ähnelt: "Fehler bei Trefferfehler: Der Prozess kann nicht auf die Datei "ExportData.db" zugreifen, da sie von einem anderen Prozess verwendet wird."

Weitere Schritte zur Problembehandlung für eDiscovery-Exporte finden Sie unter ["Beheben allgemeiner eDiscovery-Probleme: Fehler](https://docs.microsoft.com/office365/troubleshoot/ediscovery/resolve-ediscovery-issues#error-hit-tolerable-error-will-retry-the-process-cannot-access-the-file-exportdatadb-because-it-is-being-used-by-another-process)beim Beheben von Trefferfehlern".
