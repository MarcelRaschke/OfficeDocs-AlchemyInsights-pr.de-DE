---
title: Beheben von Fehlern bei der eDiscovery-Aufbewahrung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 71dec5d511eb27277ade7885526e422931623c9b
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61946626"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Beheben von Fehlern bei der eDiscovery-Aufbewahrung

Gibt es Probleme bei der eDiscovery-Aufbewahrung? Hier finden Sie einige bewährte Methoden, die Sie berücksichtigen sollten:

- Überprüfen Sie den Verteilungsstatus der Aufbewahrung.  Wenn der Status auf **Ein (Ausstehend)** oder **Aus (Ausstehend)** festgelegt ist, warten Sie, bis die Aufbewahrungsverteilung abgeschlossen ist.
- Führen Sie eDiscovery-Aufbewahrungsaktualisierungen in einer einzelnen Massenanforderung zusammen, statt die Richtlinie für jede Transaktion einzeln zu aktualisieren.
- Führen Sie `Set-CaseHoldPolicy <policyname> -RetryDistribution` im Security and Compliance Center PowerShell aus. Details finden Sie unter [Herstellen einer Verbindung mit der Security und Compliance Center-PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell).

Schritte zum Überprüfen dieser Einstellungen und weitere bewährte Methoden für die Verringerung und Behebung von Problemen bei der eDiscovery-Aufbewahrung finden Sie unter [Beheben von Fehlern bei der eDiscovery-Aufbewahrung](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors).
Informationen zur Problembehandlung bei anderen häufigen eDiscovery-Problemen finden Sie unter [Untersuchung, Problembehandlung und Lösung häufiger eDiscovery-Probleme](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
