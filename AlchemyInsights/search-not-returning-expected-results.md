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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 53fbf490f3a6aac3719a766a884e77d0cad7e5ae
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63181040"
---
# <a name="content-search-not-returning-expected-results"></a>Inhaltssuche gibt keine erwarteten Ergebnisse zurück

Beim Ausführen von Inhaltssuchen im Microsoft 365 Security & Compliance Center erhalten Sie möglicherweise unerwartete Suchergebnisse. Berücksichtigen Sie die folgenden Punkte, die sich auf Ihre Suchergebnisse auswirken können:

- **Inhaltsspeicherorte und Suchbedingungen**: Stellen Sie sicher, dass Sie die richtigen Inhaltsspeicherorte und Suchbedingungen ausgewählt haben. Wenn Sie eine umfangreiche Suche (mit vielen Speicherorten) ausgeführt haben, sollten Sie sie in mehrere Suchvorgänge aufteilen.

- **Teilweise indizierte Elemente**:  [Teilweise indizierte Elemente](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) aus Postfächern sind in den geschätzten Suchergebnissen enthalten. Teilweise indizierte Elemente von Websites in SharePoint und OneDrive sind jedoch nicht in der Suchvorkalkulation enthalten.

- **Suchfehler**: Beim Durchsuchen einer großen Anzahl von Postfächern (über 100.000 Postfächer) erhalten Sie möglicherweise Suchfehler mit Fehlercodes wie CS008-009 und CS012-002). Wiederholen Sie in diesem Fall die Suche nur nach den fehlerhaften Inhaltsspeicherorten. Weitere Informationen finden Sie  [in diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
