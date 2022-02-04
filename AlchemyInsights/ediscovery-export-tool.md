---
title: eDiscovery-Exporttool
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
  - 263
  - 928
  - 1100001
  - 3100022
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
---

# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kann das eDiscovery-Exporttool nicht installiert oder ausgeführt werden?

Wenn Sie das eDiscovery-Exporttool nicht installieren oder ausführen können, um Suchergebnisse herunterzuladen, überprüfen Sie Folgendes:
  
- Der computer, den Sie verwenden, erfüllt die folgenden Voraussetzungen:

  - 32- oder 64-Bit-Versionen von Windows 7 und höher

  - Microsoft .NET Framework 4.7

  - Unterstützter Browser:

  - Microsoft Edge

    Oder

  - Internet Explorer 10 und höher

    Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.

- Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, der **\* blob.core.windows.net** ist (der Platzhalter stellt einen eindeutigen Bezeichner für Ihren Exportauftrag dar).

- Ihnen wird die Exportrolle im Microsoft 365 Security &amp; Compliance Center zugewiesen. Standardmäßig wird diese Rolle nur der Rollengruppe "eDiscovery-Manager" zugewiesen. Weitere Informationen finden Sie unter [Zuweisen von eDiscovery-Berechtigungen.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Weitere Informationen finden Sie unter Exportieren von [Inhaltssuchergebnissen.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Wenn Sie mehr als 100.000 Postfächer exportieren, müssen Sie die folgende PowerShell verwenden, um die Exportergebnisse herunterzuladen: [Exportieren von Ergebnissen aus mehr als 100.000 Postfächern.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results%23exporting-results-from-more-than-100000-mailboxes)