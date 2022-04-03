---
title: eDiscovery-Fallsperre im Status "PendingDeletion" hängen geblieben
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9010644"
- "16952"
ms.date: 03/31/2022
ms.openlocfilehash: 79065fcc740ba15603718fe825e6d1abf8e30684
ms.sourcegitcommit: 01c1bc49e5972cd4a4aec6426774d9ff0ec99ae1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/31/2022
ms.locfileid: "64592551"
---
# <a name="ediscovery-case-hold-stuck-in-pendingdeletion-state"></a>eDiscovery-Fallsperre im Status "PendingDeletion" hängen geblieben

Wenn Sie die [eDiscovery-Fallsperre](https://docs.microsoft.com/microsoft-365/compliance/create-ediscovery-holds) oder [Aufbewahrungsrichtlinie](https://docs.microsoft.com/microsoft-365/compliance/retention) nicht entfernen können, weil sie in einem **Zustand "PendingDeletion** " hängen bleibt, stellen Sie eine Verbindung mit [Security and Compliance Center PowerShell her,](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps&preserve-view=true) und führen Sie die folgenden Schritte aus:

1. Führen Sie den `RetryDistribution` Parameter für die Richtlinie aus.

    Für eDiscovery-Fallarchive:

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

Weitere Informationen zur Problembehandlung von eDiscovery-Haltebereichsproblemen finden Sie unter ["Behandeln allgemeiner eDiscovery-Probleme"](https://docs.microsoft.com/office365/troubleshoot/ediscovery/resolve-ediscovery-issues).
