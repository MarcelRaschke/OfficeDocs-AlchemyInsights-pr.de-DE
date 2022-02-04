---
title: Behandeln von Problemen mit dem Öffnen mit Explorer
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 918b4982c55a0f9b812ed96dea1216191cac5534
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61937659"
---
# <a name="fix-problems-with-open-with-explorer"></a>Beheben von Problemen mit "Öffnen mit Explorer"

Beheben sie allgemeine Probleme beim Öffnen einer Dokumentbibliothek in SharePoint oder OneDrive mithilfe des Befehls **"Mit Explorer öffnen":** 
  
- Verwenden Sie Internet Explorer 10 oder Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Das Öffnen mit Explorer** ist in allen Browsern außer Internet Explorer deaktiviert. 
    
- **Open with Explorer** is not available in the modern experience for SharePoint libraries. Verwenden Sie stattdessen **die Ansicht im Datei-Explorer.** Wählen  Sie \> **im Datei-Explorer ansichtsoptionen anzeigen** aus. Ansicht im Datei-Explorer ist nicht kompatibel mit Microsoft Edge, Google Chrome, Firefox und anderen. **Ansicht im Datei-Explorer** nur in Internet Explorer verfügbar. 
    
- Stellen Sie sicher, dass der WebClient-Dienst ausgeführt wird. Geben Sie im Suchfeld Windows ausführen ein, wählen Sie die Desktop-App ausführen aus, geben Sie "services.msc" ein, und drücken Sie dann die EINGABETASTE. Scrollen Sie nach unten zum WebClient-Dienst, und stellen Sie sicher, dass in der Spalte **"Status"** "Ausgeführt" angezeigt wird. Wenn dies nicht der Fall ist, doppelklicken Sie auf den Dienst, klicken Sie auf **"Start"** und dann auf **"OK".** (Möglicherweise müssen Sie zuerst den Dienst aktivieren, indem Sie im Feld **"Starttyp"** entweder **"Manuell"** oder **"Automatisch"** auswählen.) 
    
**Hinweis:** Das Öffnen einer Bibliothek im Datei-Explorer ist praktisch, wenn Sie mehrere Dateien und Ordner einmal kopieren oder verschieben müssen. Wenn Sie jedoch regelmäßig in der Bibliothek arbeiten möchten, empfehlen wir die Synchronisierung. Informationen zum Beheben von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Öffnen im Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Informationen zum Einrichten der Synchronisierung finden Sie unter ["Synchronisieren SharePoint Dateien mit dem neuen OneDrive-Synchronisation-Client".](https://go.microsoft.com/fwlink/?linkid=871666)
  
Weitere Informationen finden Sie im Artikel ["Verwenden des Befehls "Mit Explorer öffnen", um Probleme in SharePoint Online zu beheben.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
