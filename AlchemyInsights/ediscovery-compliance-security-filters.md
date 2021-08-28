---
title: Während der Inhaltssuche/-export werden keine Ergebnisse zurückgegeben.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101265"
---
# <a name="no-results-returned-during-content-searchexport"></a>Während der Inhaltssuche/-export werden keine Ergebnisse zurückgegeben.

Wenn Probleme mit den folgenden eDiscovery-Szenarien auftreten:

- Inhaltssuche/-export gibt keine Daten oder unerwartete Daten zurück
- eDiscovery-Suche oder -Export schlägt fehl

Dies kann auf bestimmte Compliancesicherheitsfilter zurückzuführen sein, die von einem bestimmten Administrator eingerichtet und nicht an alle Administratoren kommuniziert wurden.

Um dies zu beheben, überprüfen Sie, ob Compliancesicherheitsfilter vorhanden sind, die diese Probleme verursachen können:

1. Verbinden zu Security and Compliance Center PowerShell
2. Führen Sie die folgenden Commandlets aus:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Weitere Informationen zu Compliancesicherheitsfiltern finden Sie unter ["Berechtigungsfilterung für die Inhaltssuche"](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
