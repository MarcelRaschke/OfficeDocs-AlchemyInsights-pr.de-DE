---
title: Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002930"
- "5611"
ms.date: 07/24/2020
ms.openlocfilehash: 3c5bacbd228d0ada22101f329befda6db3d5d65e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66327812"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Diagramm mit einer unterschiedlichen Anzahl von Datensätzen im Raster

**Symptom**

Wenn Sie bei einem Diagramm auf der Dashboard-Seite auf das Diagramm „...“ und dann auf „Datensätze anzeigen“ klicken, gelangen Sie auf die Rasterseite, auf der Sie alle Datensätze sehen können, wobei sich manchmal die Anzahl der Datensätze ändert.

**Ursache**

Dies ist auf die unterschiedlichen Ansichten zwischen dem Diagramm auf der ursprünglichen Dashboardseite und dem Diagramm auf der Rasterstartseite zurückzuführen.  

**Lösung**

1. Überprüfen Sie die Ansicht auf der ursprünglichen Seite und der Ansicht im Raster, um zu sehen, ob Sie anders sind.
2. Ändern Sie die Ansicht im Raster so, dass sie der Ansicht auf der ursprünglichen Seite entspricht.
3. Wenn die richtige Darstellung nicht gefunden werden kann, bedeutet dies normalerweise, dass die Ansicht im App-Designer nicht aktiviert ist.
4. Wechseln Sie zum App-Designer der jeweiligen App, wählen Sie die Entität und deren Ansichten aus, überprüfen Sie die Ansicht, die Sie aktivieren, speichern, veröffentlichen und schließen möchten.
5. Aktualisieren Sie die Seite.