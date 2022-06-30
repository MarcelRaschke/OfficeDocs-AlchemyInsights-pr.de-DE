---
title: Die Freigabe für externe Benutzer funktioniert nicht
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
ms.openlocfilehash: 9512d44a7b905667e6ad4d99a05411b283091eb7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66425506"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Beheben von Problemen beim Freigeben von SharePoint-Inhalten für externe Benutzer

Stellen Sie sicher, dass die externe Freigabe für Ihre Organisation aktiviert ist:
  
1. Wechseln Sie im [Microsoft 365 Admin Center zur Seite "Dienste-Add-Ins&amp;](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)", und klicken Sie auf **"Websites"**.
    
2. Stellen Sie sicher, dass die Einstellung auf "Ein" aktiviert ist. Wenn "Nur vorhandene externe Benutzer" ausgewählt ist, stellen Sie sicher, dass der externe Benutzer in der Microsoft 365 Admin Center aufgeführt ist.
    
Stellen Sie sicher, dass die externe Freigabe für die Website aktiviert ist. Für eine klassische Websitesammlung:
  
1. Klicken Sie im neuen SharePoint Admin Center im linken Bereich auf **Websites**.
    
2. Wählen Sie die Website oder Websites aus, und klicken Sie im Menüband auf **"Freigeben"**.
    
Für eine Teamwebsite, die zu einer Microsoft 365-Gruppe gehört, oder für eine Kommunikationswebsite:
  
- Diese neuen Websitetypen haben dieselbe Freigabeeinstellung wie Ihre organisationsweite Einstellung, es sei denn, die organisationsweite Einstellung ermöglicht das Freigeben von Dateien über Links, für die keine Anmeldung erforderlich ist. In diesem Fall erlauben die Websites die Freigabe für neue und vorhandene externe Benutzer, die sich anmelden. Um die Einstellung für bestimmte Websites zu ändern, verwenden Sie das neue SharePoint Admin Center oder PowerShell. [Weitere Informationen](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Hinweis**: Die Einstellung für die externe Freigabe für jede Website kann restriktiver sein als ihre organisationsweite Einstellung, aber nicht eingeschränkter als die organisationsweite Einstellung. 
  

