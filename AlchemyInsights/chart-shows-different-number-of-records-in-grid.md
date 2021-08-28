---
title: Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950079"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster

**Symptom**

Wenn Sie bei einem Diagramm auf der Dashboardseite auf das Diagramm „...“ klicken und auf „Datensätze anzeigen“ klicken, navigieren Sie zur Rasterseite, um alle Datensätze zu sehen. Manchmal ändert sich die Anzahl der Datensätze.

**Ursache**

Dies ist auf die unterschiedlichen Ansichten zwischen dem Diagramm auf der ursprünglichen Dashboardseite und dem Diagramm auf der Rasterstartseite zurückzuführen.  

**Lösung**

1. Überprüfen Sie die Ansicht auf der ursprünglichen Seite und der Ansicht im Raster, um zu sehen, ob Sie anders sind.
2. Ändern Sie die Ansicht im Raster so, dass sie der Ansicht auf der ursprünglichen Seite entspricht.
3. Wenn die richtige Darstellung nicht gefunden werden kann, bedeutet dies normalerweise, dass die Ansicht im App-Designer nicht aktiviert ist.
4. Wechseln Sie zum App-Designer der jeweiligen App, wählen Sie die Entität und deren Ansichten aus, überprüfen Sie die Ansicht, die Sie aktivieren, speichern, veröffentlichen und schließen möchten.
5. Aktualisieren Sie die Seite.