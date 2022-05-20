---
title: eDiscovery-Exporttool
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 88ccc1d79faeaa5516ee5df1193f385b260d3ca4
ms.sourcegitcommit: 654bbec12ffc98760723fe13ad3f69b9cff95a72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/20/2022
ms.locfileid: "65611761"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kann das eDiscovery-Exporttool nicht installiert oder ausgeführt werden?

Wenn Sie das eDiscovery-Exporttool nicht installieren oder ausführen können, um Suchergebnisse herunterzuladen, überprüfen Sie Folgendes:
  
- Der von Ihnen genutzte Computer erfüllt die folgenden Voraussetzungen:

  - 32- oder 64-Bit-Versionen von Windows 7 und höher

  - Microsoft .NET Framework 4.7

  - Unterstützter Browser:

    - Microsoft Edge

      Informationen zum Aktivieren ClickOnce Unterstützung in Microsoft Edge finden [Sie unter Verwenden des eDiscovery-Exporttools in Microsoft Edge](https://docs.microsoft.com/microsoft-365/compliance/configure-edge-to-export-search-results).

      Oder

    - Internet Explorer 10 und höher

      Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.

- Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, **der blob.core.windows.net ist\*** (der Platzhalter stellt einen eindeutigen Bezeichner für Ihren Exportauftrag dar).

- Ihnen wird die Rolle "Exportieren" im Microsoft 365 Security &amp; Compliance Center zugewiesen. Standardmäßig wird diese Rolle nur der Rollengruppe "eDiscovery-Manager" zugewiesen. Siehe [Zuweisen von eDiscovery-Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Weitere Informationen finden Sie unter [Exportieren von Inhaltssuchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Wenn Sie mehr als 100 KB Postfächer exportieren, müssen Sie die folgende Powershell verwenden, um die Exportergebnisse herunterzuladen:  [Exportieren von Ergebnissen aus mehr als 100 KB Postfächern](https://docs.microsoft.com/microsoft-365/compliance/export-search-results#exporting-results-from-more-than-100000-mailboxes).