---
title: Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 6cf6cd7fdef66abee251c7a1dab3c22b70cf3bc5
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61954245"
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