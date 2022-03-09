---
title: Freigabe für externe Benutzer funktioniert nicht
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
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4c6781efd282bb7795b8f704c3a0ecfe2e83c54f
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63292251"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Beheben von Problemen bei der Freigabe SharePoint Inhalten für externe Benutzer

Stellen Sie sicher, dass die externe Freigabe für Ihre Organisation aktiviert ist:
  
1. Wechseln Sie im [Microsoft 365 Admin Center zur Seite "Dienste-Add-Ins&amp;](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)", und klicken Sie auf **"Websites**".
    
2. Stellen Sie sicher, dass die Einstellung auf "Ein" aktiviert ist. Wenn "Nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer im Microsoft 365 Admin Center aufgeführt ist.
    
Stellen Sie sicher, dass die externe Freigabe für die Website aktiviert ist. Für eine klassische Websitesammlung:
  
1. Klicken Sie im neuen SharePoint Admin Center im linken Bereich auf **Websites**.
    
2. Wählen Sie die Website oder Websites aus, und klicken Sie auf dem Menüband auf **"Freigabe**".
    
Für eine Teamwebsite, die zu einer Microsoft 365 Gruppe oder einer Kommunikationswebsite gehört:
  
- Diese neuen Websitetypen haben die gleiche Freigabeeinstellung wie Ihre organisationsweite Einstellung, es sei denn, die organisationsweite Einstellung ermöglicht das Freigeben von Dateien über Links, für die keine Anmeldung erforderlich ist. In diesem Fall ermöglichen die Websites die Freigabe für neue und vorhandene externe Benutzer, die sich anmelden. Um die Einstellung für bestimmte Websites zu ändern, verwenden Sie das neue SharePoint Admin Center oder PowerShell. [Weitere Informationen](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Hinweis**: Die Einstellung für die externe Freigabe für jede Website kann restriktiver sein als ihre organisationsweite Einstellung, aber nicht weniger restriktiv als die organisationsweite Einstellung. 
  

