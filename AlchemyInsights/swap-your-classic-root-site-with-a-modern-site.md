---
title: Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 04cb5a47f5a7566e32f792753f0aebbd995abee0
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61942459"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.

Wenn Ihre Umgebung vor April 2019 eingerichtet wurde, können Sie Ihre Stammwebsite mithilfe von Microsoft PowerShell in eine moderne Website ändern:

- Wenn Sie über eine andere Website verfügen, die Sie als Stammwebsite verwenden möchten, können Sie die Stammwebsite durch diese ersetzen [(austauschen).](https://docs.microsoft.com/sharepoint/modern-root-site)

  - Verwenden Sie [Invoke-SPOSiteSwap,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps&preserve-view=true) um den Standort eines Standorts mit einem anderen Standort auszutauschen, während Sie den ursprünglichen Standort archivieren. Verfügbar für Teamwebsite (nicht mit einer Gruppe verbunden) und Kommunikationswebsite.

- In Kürze werden zusätzliche Funktionen eingeführt, mit denen Sie weiterhin den Inhalt der Website verwenden, aber die vorhandene Website in eine Kommunikationswebsite konvertieren können.

**Wichtig:** Diese Funktionen werden schrittweise eingeführt. Fahren Sie fort, um das Nachrichtencenter auf Updates zu überprüfen.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austauschen von Websites

- Die Zielwebsite gibt möglicherweise einen HTTP 404-Fehler (Nicht gefunden) für einen kurzen Zeitraum zurück.
- Inhalte müssen erneut durchforsst werden, um den Suchindex zu aktualisieren. Es ist kein manueller Schritt erforderlich – dies erfolgt automatisch.
- Alles, was von "statischen" Links abhängig ist (z. B. Dateisynchronisierung und OneNote Dateien), muss manuell korrigiert werden.
- Wenn die Quellwebsite eine Nachrichtenwebsite der Organisation war, aktualisieren Sie die URL. Abrufen einer Liste aller Nachrichtenwebsites der Organisation.
- Project Serverwebsites müssen möglicherweise überprüft werden, um sicherzustellen, dass sie weiterhin korrekt zugeordnet sind.
