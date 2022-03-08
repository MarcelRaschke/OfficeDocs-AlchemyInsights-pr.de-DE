---
title: Verwenden von Microsoft Edge basierend auf Chromium Browsern für den EDiscovery-Export
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: ec48e2ceffefd45b57d56ca42dd137c811234147
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63281033"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Verwenden von Microsoft Edge basierend auf Chromium Browsern für den EDiscovery-Export

Aufgrund einer kürzlichen Änderung ist Microsoft Edge Browsern nicht mehr ClickOnce Standardmäßig aktiviert. Um das Microsoft 365 eDiscovery-Exporttool weiterhin zu verwenden, müssen Sie entweder Microsoft Internet Explorer verwenden oder ClickOnce Support in Microsoft Edge aktivieren. 

So aktivieren Sie ClickOnce Support in Microsoft Edge basierend auf Chromium: 
1. Besuchen Sie in Ihrem Microsoft Edge Browser edge://flags/#edge-click-once.
2. Ändern Sie für die Option „ClickOnce-Unterstützung“ den Wert von **Standard** oder **Deaktiviert** in **Aktiviert**. 
3. Wählen Sie am unteren Rand des Browserfensters **"Neu starten**" aus. <br>
 Die Änderung wird nach dem Neustart Microsoft Edge wirksam. 

Informationen dazu und Schritte zum Installieren des Exporttools finden Sie unter: [ Exportieren von Inhaltssuchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).