---
title: Verwenden von Microsoft Edge basierend auf Chromium Browsern für den EDiscovery-Export
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 76a4ab2e67d1f82b1b04b6aae14c3ae91fc464b2
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62725137"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Verwenden von Microsoft Edge basierend auf Chromium Browsern für den EDiscovery-Export

Aufgrund einer kürzlichen Änderung ist Microsoft Edge Browsern ClickOnce Unterstützung nicht mehr standardmäßig aktiviert. Um weiterhin das Microsoft 365 eDiscovery-Exporttool verwenden zu können, müssen Sie entweder Microsoft Internet Explorer verwenden oder ClickOnce Support in Microsoft Edge aktivieren. 

So aktivieren Sie ClickOnce Support in Microsoft Edge basierend auf Chromium: 
1. Besuchen Sie in Ihrem Microsoft Edge Browser edge://flags/#edge-click-once.
2. Ändern Sie für die Option „ClickOnce-Unterstützung“ den Wert von **Standard** oder **Deaktiviert** in **Aktiviert**. 
3. Wählen Sie am unteren Rand des Browserfensters **"Neu starten**" aus. <br>
 Die Änderung wird nach dem Neustart Microsoft Edge wirksam. 

Informationen dazu und Schritte zum Installieren des Exporttools finden Sie unter: [ Exportieren von Inhaltssuchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).