---
title: eDiscovery-Fall im Status "PendingDeletion" hängen geblieben
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9010644"
- "16952"
ms.date: 03/31/2022
ms.openlocfilehash: 8b6a941e92452c8bdc2048ecaa0a2a365e52bb1f
ms.sourcegitcommit: 5cdb7885e5ac2787c6616101ee1bc7fb23809427
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2022
ms.locfileid: "65219716"
---
# <a name="ediscovery-case-hold-stuck-in-pendingdeletion-state"></a>eDiscovery-Fall im Status "PendingDeletion" hängen geblieben

Wenn Sie ihre [eDiscovery-Fallsperre](https://docs.microsoft.com/microsoft-365/compliance/create-ediscovery-holds) oder [Aufbewahrungsrichtlinie](https://docs.microsoft.com/microsoft-365/compliance/retention) nicht entfernen können, weil sie im Status **"PendingDeletion** " hängen bleibt, stellen Sie eine Verbindung mit [Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps&preserve-view=true) her, und führen Sie die folgenden Schritte aus:

1. Führen Sie den `RetryDistribution` Parameter für die Richtlinie aus.

    Für eDiscovery-Fallspeicher gilt Folgendes:

    ```PowerShell
    Set-CaseHoldPolicy <policyname> -RetryDistribution
    ```

    Für Aufbewahrungsrichtlinien:

    ```PowerShell
    Set-RetentionCompliancePolicy <policyname> -RetryDistribution

2. Try to delete the policy using PowerShell with the `-ForceDeletion` parameter:

    For eDiscovery case holds, use the [`Remove-CaseHoldPolicy`](https://docs.microsoft.com/powershell/module/exchange/remove-caseholdpolicy?view=exchange-ps&preserve-view=true) cmdlet:

    ```PowerShell
    Remove-CaseHoldPolicy <policyname> -ForceDeletion
    ```

    Verwenden Sie für Aufbewahrungsrichtlinien das [`Remove-RetentionCompliancePolicy`](https://docs.microsoft.com/powershell/module/exchange/remove-retentioncompliancepolicy?view=exchange-ps&preserve-view=true) Cmdlet:

    ```PowerShell
    Remove-RetentionCompliancePolicy <policyname> -ForceDeletion
    ```

Weitere Informationen zur Problembehandlung bei eDiscovery-Haltebereichsproblemen finden Sie [unter Problembehandlung bei häufig auftretenden eDiscovery-Problemen](https://docs.microsoft.com/office365/troubleshoot/ediscovery/resolve-ediscovery-issues).
