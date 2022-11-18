---
title: "\"Mit Explorer öffnen\" funktioniert nicht"
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
ms.openlocfilehash: 3345ac9bf1085253afc35b679876824c12123476
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66349815"
---
# <a name="open-with-explorer-isnt-working"></a>"Mit Explorer öffnen" funktioniert nicht

Wenn **"Mit Explorer** öffnen" oder **"Anzeigen in Explorer**" nicht funktioniert, stellen Sie sicher, dass der WebClient-Dienst auf **"Ausführen"** festgelegt ist, indem Sie die folgenden Schritte ausführen. Das Öffnen einer SharePoint- oder OneDrive-Bibliothek kann beispielsweise sehr lange dauern, wenn der Dienst nicht ausgeführt wird. 
  
1. Geben Sie im Windows-Suchfeld "Run" ein, wählen Sie die Desktop-App "Run" aus, geben Sie "services.msc" ein, und drücken Sie dann die **EINGABETASTE**.
    
2. Scrollen Sie nach unten zum WebClient-Dienst, und überprüfen Sie die Spalte **"Status"** . Wenn der WebClient-Dienststatus nicht **ausgeführt** wird, doppelklicken Sie auf den Dienst, klicken Sie auf **"Start**", und klicken Sie dann auf **"OK**". Aktivieren Sie den Dienst bei Bedarf, indem Sie im **Feld "Starttyp**" entweder "**Manuell**" oder "**Automatisch**" auswählen. 
    
**Hinweis**: Informationen zum Beheben von Problemen beim Öffnen in Explorer finden Sie [unter "Im Explorer öffnen"](https://go.microsoft.com/fwlink/?linkid=871665). Erkunden Sie die Synchronisierung als bessere Alternative: [Synchronisieren Sie SharePoint-Dateien mit dem neuen OneDrive-Synchronisation-Client](https://go.microsoft.com/fwlink/?linkid=871666). 
  

