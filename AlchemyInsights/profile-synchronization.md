---
title: Profilsynchronisierung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: be2d5598fabfda212939a84ea6cd76ccbde6a8a0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66419062"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wann werden meine Profiländerungen mit der SharePoint-Benutzerprofilanwendung synchronisiert?

SharePoint Online verwendet den Active Directory-Importzeitgeberauftrag (AD-Import), um Benutzer und Gruppen in die Benutzerprofilanwendung zu importieren. 
  
1. AD Import synchronisiert Änderungen aus dem SharePoint Online-Verzeichnisspeicher mit der Benutzerprofilanwendung. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.
    
**Hinweis**: Die Zeit, die für die Ausführung des Auftrags benötigt wird, hängt von der Anzahl der Änderungen ab, die verarbeitet werden müssen. Eine große Anzahl von Änderungen dauert länger. Die Service Level Agreement (SLA) besagt, dass eine Änderung an einem Benutzer im SharePoint Online-Verzeichnis in der Benutzerprofilanwendung in 24 Stunden widergespiegelt wird. 
  
[Weitere Informationen zur Benutzerprofilsynchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

