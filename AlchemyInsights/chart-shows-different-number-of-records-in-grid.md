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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 189088b3435ca12111d133d525f2e3090cafac05
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63094258"
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