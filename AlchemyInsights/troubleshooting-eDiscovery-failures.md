---
title: 1490-troubleshooting-eDiscovery-failures
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3200003"
- "1490"
ms.date: 04/21/2020
ms.openlocfilehash: b185f24c7ae5ff3a700e1c3a5d54476c56278d28
ms.sourcegitcommit: 5058f004f549ba7ac2b4843429b385287456a9c7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2022
ms.locfileid: "65062639"
---
# <a name="troubleshoot-content-search-errors"></a>Behandeln von Fehlern bei der Inhaltssuche

Treten Beim Exportieren von Suchergebnissen Probleme mit der Inhaltssuche auf oder erhalten Sie Fehler?
Erhalten Sie beispielsweise Folgendes, wenn Sie Suchvorgänge ausführen?

- CS007-, CS008- oder CS012-Fehler
- Serverbeschäftigt/Timeoutfehler
- Anwendungsfehler
- Der Speicherort *username@domain.com* ist mehrdeutig.

Oder erhalten Sie Exportfehler, wenn Sie Ergebnisse aus einer großen Anzahl (über 100.000) postfächern durchsuchen oder exportieren?

Wiederholen Sie bei diesen Fehlern die Suche nach den fehlerhaften Inhaltsspeicherorten, oder aktualisieren Sie die Suche, indem Sie die Komplexität der Suchabfrage verringern. Eine Platzhaltersuche könnte beispielsweise zu viele Ergebnisse zurückgeben, die das System verarbeiten kann, was zu einem CS007-Fehler führt.

Weitere Informationen finden Sie unter ["Wiederholen einer Inhaltssuche", um einen Inhaltsspeicherortfehler zu beheben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) oder [häufige eDiscovery-Probleme zu untersuchen, zu beheben und zu beheben](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

Wenn Sie mehr als 100 KB Postfächer exportieren, müssen Sie die Exportergebnisse herunterladen. Ausführliche Informationen finden [Sie unter Exportieren von Inhaltssuchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
