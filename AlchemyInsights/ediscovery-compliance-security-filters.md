---
title: Während der Inhaltssuche/des Inhaltsexports werden keine Ergebnisse zurückgegeben.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3200003"
- "7534"
ms.openlocfilehash: 9e824f9c74fb0ee303ffe6035f5a59a5a6ec22f4
ms.sourcegitcommit: 24c826da93a5c8a9b07817421214b5ac4ba81465
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2022
ms.locfileid: "67883402"
---
# <a name="no-results-returned-during-content-searchexport"></a>Während der Inhaltssuche/des Inhaltsexports werden keine Ergebnisse zurückgegeben.

Wenn Probleme mit den folgenden eDiscovery-Szenarien auftreten:

- Inhaltssuche/-export gibt keine Daten oder unerwartete Daten zurück.
- eDiscovery-Suche oder -Export schlägt fehl

Dies kann auf bestimmte Compliancesicherheitsfilter zurückzuführen sein, die von einem bestimmten Administrator eingerichtet wurden, aber nicht allen Administratoren mitgeteilt wurden.

Um dies zu beheben, überprüfen Sie, ob Compliancesicherheitsfilter vorhanden sind, die möglicherweise die folgenden Probleme verursachen:

1. Herstellen einer Verbindung mit PowerShell im Security and Compliance Center
2. Führen Sie die folgenden Cmdlets aus:

    ```PowerShell
    $org = "yourdomain.com"
    ```

    ```PowerShell
    Get-ComplianceSecurityFilter -Organization $org
    ```

Weitere Informationen zu Compliancesicherheitsfiltern finden Sie unter [Berechtigungsfilterung für die Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search).
