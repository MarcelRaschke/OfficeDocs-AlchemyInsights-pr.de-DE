---
title: Verwenden von Microsoft Edge basierend auf Chromium Browsern für den Ediscovery-Export
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100022"
- "3473"
ms.openlocfilehash: ecd38e391a3ac527c1b72100eec8252a5f27a836
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66509803"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Verwenden von Microsoft Edge basierend auf Chromium Browsern für den Ediscovery-Export

Aufgrund einer kürzlich vorgenommenen Änderung ist die ClickOnce-Unterstützung für Microsoft Edge-Browser standardmäßig nicht mehr aktiviert. Um das Microsoft 365 eDiscovery-Exporttool weiterhin zu verwenden, müssen Sie entweder Microsoft Internet Explorer verwenden oder den ClickOnce-Support in Microsoft Edge aktivieren. 

So aktivieren Sie den ClickOnce-Support in Microsoft Edge basierend auf Chromium: 
1. Besuchen Sie in Ihrem Microsoft Edge-Browser edge://flags/#edge-click-once.
2. Ändern Sie für die Option „ClickOnce-Unterstützung“ den Wert von **Standard** oder **Deaktiviert** in **Aktiviert**. 
3. Wählen Sie unten im Browserfenster " **Neu starten**" aus. <br>
 Die Änderung wird nach dem Neustart von Microsoft Edge wirksam. 

Informationen hierzu und die Schritte zum Installieren des Exporttools finden Sie unter: [ Exportieren der Ergebnisse der Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).