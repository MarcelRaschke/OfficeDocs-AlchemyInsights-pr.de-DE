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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 54b1a6ca018e7872f68dae22bcb3751799f97142
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63210488"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.

Wenn Ihre Umgebung vor April 2019 eingerichtet wurde, können Sie Ihre Stammwebsite mithilfe von Microsoft PowerShell in eine moderne Website ändern:

- Wenn Sie über eine andere Website verfügen, die Sie als Stammwebsite verwenden möchten, können Sie [die Stammwebsite](https://docs.microsoft.com/sharepoint/modern-root-site) durch diese ersetzen (austauschen).

  - Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps&preserve-view=true) , um den Standort eines Standorts mit einem anderen Standort auszutauschen, während Sie den ursprünglichen Standort archivieren. Verfügbar für Teamwebsite (nicht mit einer Gruppe verbunden) und Kommunikationswebsite.

- In Kürze werden zusätzliche Funktionen eingeführt, mit denen Sie weiterhin den Inhalt der Website verwenden, aber die vorhandene Website in eine Kommunikationswebsite konvertieren können.

**Wichtig**: Diese Funktionen werden schrittweise eingeführt. Fahren Sie fort, um das Nachrichtencenter auf Updates zu überprüfen.

## <a name="known-issues-with-swapping-sites"></a>Bekannte Probleme beim Austauschen von Websites

- Die Zielwebsite gibt möglicherweise einen HTTP 404-Fehler (Nicht gefunden) für einen kurzen Zeitraum zurück.
- Inhalte müssen erneut durchforsst werden, um den Suchindex zu aktualisieren. Es ist kein manueller Schritt erforderlich – dies erfolgt automatisch.
- Alles, was von "statischen" Links abhängig ist (z. B. Dateisynchronisierung und OneNote Dateien), muss manuell korrigiert werden.
- Wenn die Quellwebsite eine Nachrichtenwebsite der Organisation war, aktualisieren Sie die URL. Abrufen einer Liste aller Nachrichtenwebsites der Organisation.
- Project Serverwebsites müssen möglicherweise überprüft werden, um sicherzustellen, dass sie weiterhin korrekt zugeordnet sind.
