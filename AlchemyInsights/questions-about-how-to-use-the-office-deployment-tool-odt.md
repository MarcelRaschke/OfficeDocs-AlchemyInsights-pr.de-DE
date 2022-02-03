---
title: Fragen zur Verwendung des Office Deployment Tool (ODT)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4973762c69967e6058097055ed4e44c85a0e70b5
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61867404"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Fragen zur Verwendung des Office Deployment Tool (ODT)

Laden Sie das Office-Bereitstellungstool aus dem [Microsoft Download Center herunter](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Führen Sie nach dem Download die selbst entpackende ausführbare Datei aus, die die ausführbare Datei (setup.exe) und eine Beispielkonfigurationsdatei (configuration.xml) für das Office-Bereitstellungstool enthält.
  
 **So schließen Sie Microsoft 365 Apps for Enterprise Produkte von Clientcomputern aus oder entfernen sie:**
  
Bei der Installation von Microsoft 365 Apps for Enterprise können Sie bestimmte Produkte ausschließen. Führen Sie dazu die Schritte für die Installation von Office mit dem ODT aus, fügen Sie jedoch das ExcludeApp-Element in der Konfigurationsdatei hinzu. Diese Konfigurationsdatei installiert beispielsweise alle Microsoft 365 Apps for Enterprise Produkte mit Ausnahme von Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

