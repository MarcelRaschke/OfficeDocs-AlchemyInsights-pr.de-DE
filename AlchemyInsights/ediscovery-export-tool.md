---
title: Microsoft Purview-eDiscovery (Premium)-Exporttool
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1100001"
- "3100022"
- "263"
- "928"
ms.date: 07/22/2022
ms.openlocfilehash: 655d49184d0e7ee9a5b58766ca02e1c8b63f7128
ms.sourcegitcommit: b7ec572b250ab6a4e140e36a64db063df3e55c24
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2022
ms.locfileid: "67070334"
---
# <a name="cant-install-or-run-the-microsoft-purview-ediscovery-premium-export-tool"></a>Kann das Microsoft Purview-eDiscovery (Premium)-Exporttool nicht installiert oder ausgeführt werden?

Wenn Sie das Microsoft Purview-eDiscovery (Premium)-Exporttool zum Herunterladen von Suchergebnissen nicht installieren oder ausführen können, überprüfen Sie Folgendes:
  
- Der von Ihnen genutzte Computer erfüllt die folgenden Voraussetzungen:

  - 32- oder 64-Bit-Versionen von Windows 7 und höher

  - Microsoft .NET Framework 4.7

  - Unterstützter Browser:

    - Microsoft Edge

      Informationen zum Aktivieren der ClickOnce-Unterstützung in Microsoft Edge finden [Sie unter Verwenden des eDiscovery-Exporttools in Microsoft Edge](https://docs.microsoft.com/microsoft-365/compliance/configure-edge-to-export-search-results).

      Oder

    - Internet Explorer 10 und höher

      Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.

- Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, **der blob.core.windows.net ist\*** (der Platzhalter stellt einen eindeutigen Bezeichner für Ihren Exportauftrag dar).

- Ihnen wird die Rolle "Exportieren" im Microsoft Purview-Complianceportal zugewiesen. Standardmäßig wird diese Rolle nur der Rollengruppe "eDiscovery-Manager" zugewiesen. Siehe [Zuweisen von eDiscovery-Berechtigungen im Complianceportal](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Weitere Informationen finden Sie unter [Exportieren von Inhaltssuchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Wenn Sie mehr als 100 KB Postfächer exportieren, müssen Sie die folgende Powershell verwenden, um die Exportergebnisse herunterzuladen:  [Exportieren von Ergebnissen aus mehr als 100 KB Postfächern](https://docs.microsoft.com/microsoft-365/compliance/export-search-results#exporting-results-from-more-than-100000-mailboxes).
