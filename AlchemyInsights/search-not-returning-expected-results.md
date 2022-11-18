---
title: 1491-search-not-returning-expected-results
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
- "1491"
ms.date: 04/21/2020
ms.openlocfilehash: e661fe438e133eaf82546b6b1df891759dc5fa05
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66399135"
---
# <a name="content-search-not-returning-expected-results"></a>Inhaltssuche gibt keine erwarteten Ergebnisse zurück

Wenn Sie Inhaltssuchen aus dem Microsoft 365 Security & Compliance Center ausführen, erhalten Sie möglicherweise unerwartete Suchergebnisse. Berücksichtigen Sie die folgenden Punkte, die sich auf Ihre Suchergebnisse auswirken können:

- **Inhaltsspeicherorte und Suchbedingungen**: Stellen Sie sicher, dass Sie die richtigen Inhaltsspeicherorte und Suchbedingungen ausgewählt haben. Wenn Sie eine große Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie sie in mehrere Suchvorgänge aufteilen.

- **Teilweise indizierte Elemente**:  [Teilweise indizierte Elemente](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten. Teilweise indizierte Elemente von Websites in SharePoint und OneDrive sind jedoch nicht in der Suchschätzung enthalten.

- **Suchfehler**: Beim Durchsuchen einer großen Anzahl von Postfächern (über 100.000 Postfächer) können Suchfehler mit Fehlercodes wie CS008-009 und CS012-002 auftreten. Wiederholen Sie in diesem Fall die Suche nur nach den fehlerhaften Inhaltsspeicherorten. Weitere Informationen finden Sie  [in diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
