---
title: Behandeln von Problemen mithilfe von "Mit Explorer öffnen"
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.date: 04/21/2020
ms.openlocfilehash: d78a347c09abe037b54438d9daca1e6cc64b6ae0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66345563"
---
# <a name="fix-problems-with-open-with-explorer"></a>Beheben von Problemen mit "Mit Explorer öffnen"

Beheben Sie häufige Probleme beim Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mithilfe des Befehls **"Mit Explorer öffnen** ": 
  
- Verwenden Sie Internet Explorer 10 oder Internet Explorer 11. **"Mit Explorer öffnen** " ist nicht kompatibel mit Microsoft Edge, Google Chrome, Firefox und anderen. **"Mit Explorer öffnen** " ist in allen Browsern außer Internet Explorer deaktiviert. 
    
- **"Mit Explorer öffnen** " ist in der modernen Benutzeroberfläche für SharePoint-Bibliotheken nicht verfügbar. Verwenden Sie **stattdessen "Ansicht in Explorer**". Wählen Sie **"Ansichtsoptionen** \> **anzeigen" in Explorer** aus. Ansicht in Explorer ist nicht kompatibel mit Microsoft Edge, Google Chrome, Firefox und anderen. **Anzeigen in Explorer** nur in Internet Explorer verfügbar. 
    
- Stellen Sie sicher, dass der WebClient-Dienst ausgeführt wird. Geben Sie im Windows-Suchfeld "Run" ein, wählen Sie die "Desktop-App ausführen", geben Sie "services.msc" ein, und drücken Sie dann die EINGABETASTE. Scrollen Sie nach unten zum WebClient-Dienst, und stellen Sie sicher, dass in der Spalte " **Status** " "Wird ausgeführt" angezeigt wird. Doppelklicken Sie andernfalls auf den Dienst, klicken Sie auf **"Start**" und dann auf **"OK**". (Möglicherweise müssen Sie den Dienst zuerst aktivieren, indem Sie im **Feld "Starttyp**" entweder "**Manuell**" oder "**Automatisch**" auswählen.) 
    
**Hinweis**: Das Öffnen einer Bibliothek in Explorer ist praktisch, wenn Sie mehrere Dateien und Ordner einmal kopieren oder verschieben müssen, aber wenn Sie regelmäßig in der Bibliothek arbeiten möchten, empfehlen wir, sie zu synchronisieren. Informationen zum Beheben von Problemen beim Öffnen in Explorer finden Sie [unter "Im Explorer öffnen"](https://go.microsoft.com/fwlink/?linkid=871665). Informationen zum Einrichten der Synchronisierung finden Sie unter [Synchronisieren von SharePoint-Dateien mit dem neuen OneDrive-Synchronisation-Client](https://go.microsoft.com/fwlink/?linkid=871666).
  
Weitere Informationen finden Sie [im Artikel "Verwenden des Befehls "Mit Explorer öffnen", um Probleme in SharePoint Online zu beheben](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
