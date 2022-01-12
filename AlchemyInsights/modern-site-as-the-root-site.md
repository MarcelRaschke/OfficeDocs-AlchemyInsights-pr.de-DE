---
title: Moderne Website als Stammwebsite
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
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
ms.openlocfilehash: 544cf6401bd5766f9977bc6d2961f16ff9802076
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862147"
---
# <a name="modern-site-as-root-site"></a>Moderne Website als Stammwebsite

Wir haben mit dem Rollout eines neuen Features begonnen, mit dem Sie [Ihre klassische Websitestammwebsite mit einer modernen Website austauschen](https://docs.microsoft.com/sharepoint/modern-root-site)können. Verwenden Sie [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps&preserve-view=true) um den Standort eines Standorts mit einem anderen Standort auszutauschen, während Sie den ursprünglichen Standort archivieren. Verfügbar für Teamwebsite (nicht mit einer Gruppe verbunden) und Kommunikationswebsite.

**Wichtig:** Löschen Sie ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen. Dies wird von Microsoft nicht unterstützt. Wenn Sie die Stammwebsite löschen, können alle SharePoint Websites in Ihrer Organisation nicht für alle Benutzer zugänglich sein, bis Sie die Website wiederherstellen oder eine neue Website unter derselben URL erstellen. Wir kommunizieren dieses Feature über das Nachrichtencenter. Sie sollten davon ausgehen, dass das Feature in Kürze in Ihrem Mandanten aktiviert ist.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austauschen von Websites
- Die Zielwebsite gibt möglicherweise einen HTTP 404-Fehler (Nicht gefunden) für einen kurzen Zeitraum zurück.
- Inhalte müssen erneut durchforsst werden, um den Suchindex zu aktualisieren. Hier ist kein manueller Schritt erforderlich, dies erfolgt automatisch.
- Alles, was von statischen Links abhängig ist (z. B. Dateisynchronisierung und OneNote Dateien), muss manuell korrigiert werden.
- Project Serverwebsites müssen möglicherweise überprüft werden, um sicherzustellen, dass sie weiterhin korrekt zugeordnet sind. 
