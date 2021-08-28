---
title: 1491-search-not-returning-expected-results
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052709"
---
# <a name="content-search-not-returning-expected-results"></a>Inhaltssuche gibt keine erwarteten Ergebnisse zurück

Wenn Sie Inhaltssuchen im Microsoft 365 Security & Compliance Center ausführen, erhalten Sie möglicherweise unerwartete Suchergebnisse. Berücksichtigen Sie die folgenden Punkte, die sich auf Ihre Suchergebnisse auswirken können:

- **Inhaltsspeicherorte und Suchbedingungen:** Stellen Sie sicher, dass Sie die richtigen Inhaltsspeicherorte und Suchbedingungen ausgewählt haben. Wenn Sie eine große Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie sie in mehrere Suchvorgänge aufteilen.

- **Teilweise indizierte Elemente:**  [Teilweise indizierte Elemente](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten. Teilweise indizierte Elemente von Websites in SharePoint und OneDrive sind jedoch nicht in der Suchvorkalkulation enthalten.

- **Suchfehler:** Beim Durchsuchen einer großen Anzahl von Postfächern (über 100.000 Postfächer) erhalten Sie möglicherweise Suchfehler mit Fehlercodes wie CS008-009 und CS012-002). Wiederholen Sie in diesem Fall die Suche nur nach den fehlerhaften Inhaltsspeicherorten. Weitere Informationen finden Sie [in diesem Artikel.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)
