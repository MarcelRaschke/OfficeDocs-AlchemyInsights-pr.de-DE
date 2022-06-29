---
title: Fragen zur Verwendung des Office-Bereitstellungstools (ODT)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 8d6a16a908c99814936fe42f8c56ce7acdd3cc7b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66362739"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Fragen zur Verwendung des Office-Bereitstellungstools (ODT)

Laden Sie das Office-Bereitstellungstool aus dem [Microsoft Download Center herunter](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Führen Sie nach dem Download die selbst entpackende ausführbare Datei aus, die die ausführbare Datei (setup.exe) und eine Beispielkonfigurationsdatei (configuration.xml) für das Office-Bereitstellungstool enthält.
  
 **So schließen Sie Microsoft 365 Apps for Enterprise Produkte von Clientcomputern aus oder entfernen sie:**
  
Bei der Installation von Microsoft 365 Apps for Enterprise können Sie bestimmte Produkte ausschließen. Führen Sie dazu die Schritte für die Installation von Office mit dem ODT aus, fügen Sie jedoch das ExcludeApp-Element in der Konfigurationsdatei hinzu. Mit dieser Konfigurationsdatei werden beispielsweise alle Microsoft 365 Apps for Enterprise Produkte mit Ausnahme von Publisher installiert:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

