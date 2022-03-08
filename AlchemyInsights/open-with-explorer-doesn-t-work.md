---
title: Öffnen mit Explorer funktioniert nicht
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7eeff8a49ceb3a8ac7f51235637f385e26c2cc42
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63283589"
---
# <a name="open-with-explorer-isnt-working"></a>Öffnen mit Explorer funktioniert nicht

Wenn **"Öffnen mit Explorer** " oder **"Ansicht" im Datei-Explorer** nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst auf **"Ausführen"** festgelegt ist, indem Sie die folgenden Schritte ausführen. Beispielsweise kann es lange dauern, bis eine SharePoint oder OneDrive Bibliothek geöffnet ist, wenn der Dienst nicht ausgeführt wird. 
  
1. Geben Sie im Suchfeld Windows ausführen ein, wählen Sie die Desktop-App ausführen, geben Sie "services.msc" ein, und drücken Sie die **EINGABETASTE**.
    
2. Scrollen Sie nach unten zum WebClient-Dienst, und überprüfen Sie die Spalte **"Status** ". Wenn der WebClient-Dienststatus nicht **ausgeführt** wird, doppelklicken Sie auf den Dienst, klicken Sie auf **"Start**" und dann auf **"OK**". Aktivieren Sie den Dienst bei Bedarf, indem Sie im Feld "**Starttyp**" entweder **"Manuell**" oder "**Automatisch**" auswählen. 
    
**Hinweis**: Informationen zum Beheben von Problemen, die im Datei-Explorer geöffnet werden, finden Sie unter [Öffnen im Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Entdecken Sie die Synchronisierung als bessere Alternative: [Synchronisieren SharePoint Dateien mit dem neuen OneDrive-Synchronisation-Client](https://go.microsoft.com/fwlink/?linkid=871666). 
  

