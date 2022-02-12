---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.openlocfilehash: c6be047cdf8127b0f820326dd03a4cda2e766d54
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62583093"
---
# <a name="troubleshoot-content-search-errors"></a>Problembehandlung bei Fehlern bei der Inhaltssuche

Treten Beim Exportieren von Suchergebnissen Probleme mit der Inhaltssuche auf oder treten Fehler auf?
Erhalten Sie beispielsweise Folgendes, wenn Sie Suchvorgänge ausführen?

- CS007-, CS008- oder CS012-Fehler
- Serverauslastungs-/Timeoutfehler
- Anwendungsfehler aufgetreten
- Die Position *username@domain.com* mehrdeutig ist

Oder erhalten Sie Exportfehler, wenn Sie Ergebnisse aus einer großen Anzahl von Postfächern (über 100.000) suchen oder exportieren?

Wiederholen Sie bei diesen Fehlern die Suche nach den fehlerhaften Inhaltsspeicherorten, oder aktualisieren Sie die Suche, indem Sie die Komplexität der Suchabfrage verringern. Beispielsweise könnte eine Platzhaltersuche zu viele Ergebnisse zurückgeben, die das System verarbeiten kann, was einen CS007-Fehler verursacht.

Weitere Informationen finden Sie unter [Retry a Content Search to resolve a content location error](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) or [Investigate, troubleshoot, and resolve common eDiscovery issues](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

Wenn Sie mehr als 100.000 Postfächer exportieren, müssen Sie die Exportergebnisse herunterladen. Ausführliche Informationen finden Sie unter ["Exportieren von Inhaltssuchergebnissen"](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
