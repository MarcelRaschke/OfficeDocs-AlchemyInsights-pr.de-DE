---
title: Öffnen mit Explorer funktioniert nicht
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321860"
---
# <a name="open-with-explorer-isnt-working"></a>Öffnen mit Explorer funktioniert nicht

Wenn **"Öffnen mit Explorer"** oder **"Ansicht" im Datei-Explorer** nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst auf **"Ausführen"** festgelegt ist, indem Sie die folgenden Schritte ausführen. Beispielsweise kann es lange dauern, bis eine SharePoint oder OneDrive Bibliothek geöffnet ist, wenn der Dienst nicht ausgeführt wird. 
  
1. Geben Sie im Suchfeld Windows Ausführen ein, wählen Sie die Desktop-App ausführen, geben Sie "services.msc" ein, und drücken Sie die **EINGABETASTE.**
    
2. Scrollen Sie nach unten zum WebClient-Dienst, und überprüfen Sie die Spalte **"Status".** Wenn der WebClient-Dienststatus nicht **ausgeführt** wird, doppelklicken Sie auf den Dienst, klicken Sie auf **"Start"** und dann auf **"OK".** Aktivieren Sie den Dienst bei Bedarf, indem Sie im Feld **"Starttyp"** entweder **"Manuell"** oder **"Automatisch"** auswählen. 
    
**Hinweis:** Informationen zum Beheben von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Öffnen im Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Entdecken Sie die Synchronisierung als bessere Alternative: [Synchronisieren sie SharePoint Dateien mit dem neuen OneDrive-Synchronisation-Client.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

