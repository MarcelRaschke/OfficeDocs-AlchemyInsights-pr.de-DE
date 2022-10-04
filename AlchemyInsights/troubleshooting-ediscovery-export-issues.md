---
title: Problembehandlung von eDiscovery-Exportproblemen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9010644"
- "2513"
ms.date: 10/04/2022
ms.openlocfilehash: 04925273009652a33c6b122b0cfb55bd7b465700
ms.sourcegitcommit: 00019315aac844f1d4068767611d4078bb3c641e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/04/2022
ms.locfileid: "68373596"
---
# <a name="troubleshooting-ediscovery-export-issues"></a>Problembehandlung von eDiscovery-Exportproblemen

Wenn Sie Probleme mit eDiscovery-Exporten haben, versuchen Sie Folgendes:

- Stellen Sie sicher, dass Sie die Anforderungen für eDiscovery-Exporte erfüllen. Weitere Informationen finden Sie unter: 
    - eDiscovery(Standard) [Exportieren und Herunterladen von Inhalten aus einem eDiscovery(Standard)-Fall](https://learn.microsoft.com/microsoft-365/compliance/export-content-in-core-ediscovery)
    - eDiscovery(Premium) [Exportieren von Falldaten in eDiscovery (Premium)](https://learn.microsoft.com/microsoft-365/compliance/exporting-data-ediscover20)
- Überprüfen Sie eDiscovery-Berechtigungen. Weitere Informationen finden Sie unter:
    - Ediscovery(Standard) [Erste Schritte mit eDiscovery(Standard)-Fällen in Microsoft Purview](https://learn.microsoft.com/microsoft-365/compliance/get-started-core-ediscovery?source=recommendations#step-2-assign-ediscovery-permissions)
    - Ediscovery(Premium) [Einrichten von eDiscovery (Premium) in Microsoft Purview](https://learn.microsoft.com/microsoft-365/compliance/get-started-with-advanced-ediscovery#step-2-assign-ediscovery-permissions)
- Überprüfen Sie eDiscovery-Exportlimiten. Weitere Informationen finden Sie unter [Limiten für die eDiscovery-Suche](https://docs.microsoft.com/microsoft-365/compliance/limits-for-content-search#export-limits).
- Bei langsamen Downloads versuchen Sie, den Export auf ein lokales Laufwerk statt auf ein Netzwerk-Laufwerk zu speichern.
- If the search is stuck or not progressing, try re-running the search and export again. Re-run searches more than 7 days old.

Weitere Informationen zur Problembehandlung bei anderen häufigen eDiscovery-Problemen finden Sie unter [Untersuchung, Problembehandlung und Lösung häufiger eDiscovery-Probleme](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

Schritte zum Überprüfen dieser Einstellungen und mehr bewährte Methoden für die Entschärfung und Behebung von Problemen bei der eDiscovery-Aufbewahrung finden Sie unter [Beheben von Fehlern bei der eDiscovery-Aufbewahrung](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors).