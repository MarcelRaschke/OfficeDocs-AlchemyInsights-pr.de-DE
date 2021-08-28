---
title: Moderne Website als Stammwebsite
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327601"
---
# <a name="modern-site-as-root-site"></a>Moderne Website als Stammwebsite

Wir haben mit dem Rollout eines neuen Features begonnen, mit dem Sie [Ihre klassische Websitestammwebsite mit einer modernen Website austauschen](https://docs.microsoft.com/sharepoint/modern-root-site)können. Verwenden Sie [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) um den Standort eines Standorts mit einem anderen Standort auszutauschen, während Sie den ursprünglichen Standort archivieren. Verfügbar für Teamwebsite (nicht mit einer Gruppe verbunden) und Kommunikationswebsite.

**Wichtig:** Löschen Sie ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen. Dies wird von Microsoft nicht unterstützt. Wenn Sie die Stammwebsite löschen, können alle SharePoint Websites in Ihrer Organisation nicht für alle Benutzer zugänglich sein, bis Sie die Website wiederherstellen oder eine neue Website unter derselben URL erstellen. Wir kommunizieren dieses Feature über das Nachrichtencenter. Sie sollten davon ausgehen, dass das Feature in Kürze in Ihrem Mandanten aktiviert ist.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austauschen von Websites
- Die Zielwebsite gibt möglicherweise einen HTTP 404-Fehler (Nicht gefunden) für einen kurzen Zeitraum zurück.
- Inhalte müssen erneut durchforsst werden, um den Suchindex zu aktualisieren. Hier ist kein manueller Schritt erforderlich, dies erfolgt automatisch.
- Alles, was von "statischen" Links abhängig ist (z. B. Dateisynchronisierung und OneNote Dateien), muss manuell korrigiert werden.
- Project Serverwebsites müssen möglicherweise überprüft werden, um sicherzustellen, dass sie weiterhin ordnungsgemäß zugeordnet sind. 
