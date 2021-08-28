---
title: Verwenden von Microsoft Edge basierend auf Chromium Browsern für den EDiscovery-Export
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: a583896b5aa8e73be5e932a729c380acc8092e73b2151647c999f9a7b69669b6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998393"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Verwenden von Microsoft Edge basierend auf Chromium Browsern für den EDiscovery-Export

Aufgrund einer kürzlichen Änderung ist Microsoft Edge Browsern nicht mehr ClickOnce Unterstützung standardmäßig aktiviert. Um weiterhin das Microsoft 365 eDiscovery-Exporttool verwenden zu können, müssen Sie entweder Microsoft Internet Explorer verwenden oder ClickOnce Support in Microsoft Edge aktivieren. 

So aktivieren Sie ClickOnce Support in Microsoft Edge basierend auf Chromium: 
1. Besuchen Sie in Ihrem Microsoft Edge Browser edge://flags/#edge-click-once.
2. Ändern Sie für die Option „ClickOnce-Unterstützung“ den Wert von **Standard** oder **Deaktiviert** in **Aktiviert**. 
3. Wählen Sie am unteren Rand des Browserfensters **"Neu starten"** aus. <br>
 Die Änderung wird nach dem Neustart Microsoft Edge wirksam. 

Informationen dazu und Schritte zum Installieren des Exporttools finden Sie unter: [Exportieren von Inhaltssuchergebnissen.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)