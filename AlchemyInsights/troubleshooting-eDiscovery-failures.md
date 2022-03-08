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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.openlocfilehash: 886121a570a2c59f8fdd47345c35b37514833a02
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63178375"
---
# <a name="troubleshoot-content-search-errors"></a>Problembehandlung bei Fehlern bei der Inhaltssuche

Treten Beim Exportieren von Suchergebnissen Probleme mit der Inhaltssuche auf oder treten Fehler auf?
Erhalten Sie beispielsweise Folgendes, wenn Sie Suchvorgänge ausführen?

- CS007-, CS008- oder CS012-Fehler
- Serverauslastungs-/Timeoutfehler
- Anwendungsfehler aufgetreten
- Die Position *username@domain.com* ist nicht eindeutig.

Oder erhalten Sie Exportfehler, wenn Sie Ergebnisse aus einer großen Anzahl von Postfächern (über 100.000) suchen oder exportieren?

Wiederholen Sie bei diesen Fehlern die Suche nach den fehlerhaften Inhaltsspeicherorten, oder aktualisieren Sie die Suche, indem Sie die Komplexität der Suchabfrage verringern. Beispielsweise könnte eine Platzhaltersuche zu viele Ergebnisse zurückgeben, die das System verarbeiten kann, was einen CS007-Fehler verursacht.

Weitere Informationen finden Sie unter [Retry a Content Search to resolve a content location error](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) or [Investigate, troubleshoot, and resolve common eDiscovery issues](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

Wenn Sie mehr als 100.000 Postfächer exportieren, müssen Sie die Exportergebnisse herunterladen. Ausführliche Informationen finden Sie unter ["Exportieren von Inhaltssuchergebnissen"](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
