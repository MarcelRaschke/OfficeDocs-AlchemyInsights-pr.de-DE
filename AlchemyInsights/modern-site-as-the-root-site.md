---
title: Moderne Website als Stammwebsite
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000265"
- "1874"
ms.date: 04/21/2020
ms.openlocfilehash: 0d661f1b568fe6799bdcec953a39ebd7689e33d7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66431950"
---
# <a name="modern-site-as-root-site"></a>Moderne Website als Stammwebsite

Wir haben mit dem Rollout eines neuen Features begonnen, mit dem Sie [Ihre klassische Websitestammwebsite mit einer modernen Website austauschen](https://docs.microsoft.com/sharepoint/modern-root-site) können. Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps&preserve-view=true) , um den Standort eines Standorts mit einem anderen Standort zu tauschen, während der ursprüngliche Standort archiviert wird. Verfügbar für Teamwebsite (nicht mit einer Gruppe verbunden) und Kommunikationswebsite.

**Wichtig**: Löschen Sie ihre klassische Stammwebsite nicht, um eine moderne Kommunikationswebsite zu erstellen. Dies wird von Microsoft nicht unterstützt. Wenn Sie die Stammwebsite löschen, kann auf alle SharePoint-Websites in Ihrer Organisation nicht für alle Benutzer zugegriffen werden, bis Sie die Website wiederherstellen oder eine neue Website unter derselben URL erstellen. Wir kommunizieren dieses Feature über das Nachrichtencenter. Sie sollten davon ausgehen, dass das Feature in Kürze in Ihrem Mandanten aktiviert wird.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austausch von Websites
- Die Zielwebsite gibt möglicherweise für einen kurzen Zeitraum den Fehler "Nicht gefunden" (HTTP 404) zurück.
- Der Inhalt muss erneut durchforstet werden, um den Suchindex zu aktualisieren. Hier ist kein manueller Schritt erforderlich, dies erfolgt automatisch.
- Alles, was von "statischen" Links abhängig ist (z. B. Dateisynchronisierung- und OneNote-Dateien), muss manuell korrigiert werden.
- Project Server-Websites müssen möglicherweise überprüft werden, um sicherzustellen, dass sie weiterhin ordnungsgemäß zugeordnet sind. 
