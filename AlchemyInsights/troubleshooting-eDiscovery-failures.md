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
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105567"
---
# <a name="troubleshoot-content-search-errors"></a>Problembehandlung bei Fehlern bei der Inhaltssuche

Treten Beim Exportieren von Suchergebnissen Probleme mit der Inhaltssuche auf oder treten Fehler auf?

Erhalten Sie beispielsweise Folgendes, wenn Sie Suchvorgänge ausführen?

- CS008- oder CS012-Fehler

- Serverauslastungs-/Timeoutfehler

- Anwendungsfehler aufgetreten

Oder erhalten Sie beim Suchen oder Exportieren von Ergebnissen aus einer großen Anzahl von Postfächern (über 100.000 Postfächer) Exportfehler?

Wiederholen Sie bei diesen Fehlertypen die Suche nach den fehlerhaften Inhaltsspeicherorten. Weitere Informationen finden Sie [in diesem Artikel.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)

Wenn Sie mehr als 100.000 Postfächer exportieren, müssen Sie die folgende PowerShell verwenden, um die Exportergebnisse herunterzuladen: [Exportieren von Ergebnissen aus mehr als 100.000 Postfächern.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
