---
title: Ersetzen Der klassischen Stammwebsite mit einer modernen Website
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000687"
- "2579"
ms.date: 04/21/2020
ms.openlocfilehash: 143334f2b98336ffd32b9c63f8dc47846116a2d7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66262415"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Ersetzen Der klassischen Stammwebsite mit einer modernen Website

Wenn Ihre Umgebung vor April 2019 eingerichtet wurde, können Sie Ihre Stammwebsite mithilfe von Microsoft PowerShell in eine moderne Website ändern:

- Wenn Sie über eine andere Website verfügen, die Sie als Stammwebsite verwenden möchten, können Sie [die Stammwebsite durch diese ersetzen (austauschen](https://docs.microsoft.com/sharepoint/modern-root-site) ).

  - Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps&preserve-view=true) , um den Standort eines Standorts mit einem anderen Standort zu tauschen, während der ursprüngliche Standort archiviert wird. Verfügbar für Teamwebsite (nicht mit einer Gruppe verbunden) und Kommunikationswebsite.

- In Kürze werden zusätzliche Funktionen eingeführt, mit denen Sie die Inhalte auf der Website weiterhin verwenden können, die vorhandene Website jedoch in eine Kommunikationswebsite konvertieren können.

**Wichtig**: Diese Funktionen werden schrittweise eingeführt. Überprüfen Sie weiterhin das Nachrichtencenter auf Updates.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austausch von Websites

- Die Zielwebsite gibt möglicherweise für einen kurzen Zeitraum den Fehler "Nicht gefunden" (HTTP 404) zurück.
- Der Inhalt muss erneut durchforstet werden, um den Suchindex zu aktualisieren. Es ist kein manueller Schritt erforderlich – dies erfolgt automatisch.
- Alles, was von "statischen" Links abhängig ist (z. B. Dateisynchronisierung- und OneNote-Dateien), muss manuell korrigiert werden.
- Wenn es sich bei der Quellwebsite um eine Nachrichtenwebsite der Organisation handelte, aktualisieren Sie die URL. Rufen Sie eine Liste aller Nachrichtenwebsites der Organisation ab.
- Project Server-Websites müssen möglicherweise überprüft werden, um sicherzustellen, dass sie weiterhin ordnungsgemäß zugeordnet sind.
