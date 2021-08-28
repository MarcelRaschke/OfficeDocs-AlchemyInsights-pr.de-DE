---
title: Profilsynchronisierung
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320708"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wann werden meine Profiländerungen mit der SharePoint Benutzerprofilanwendung synchronisiert?

SharePoint Online verwendet den Active Directory-Importzeitgeberauftrag (AD Import), um Benutzer und Gruppen in die Benutzerprofilanwendung zu importieren. 
  
1. Der AD-Import synchronisiert Änderungen aus dem SharePoint Onlineverzeichnis Store mit der Benutzerprofilanwendung. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.
    
**Hinweis:** Die Zeit, für die der Auftrag ausgeführt werden muss, hängt von der Anzahl der zu verarbeitenden Änderungen ab. Eine große Anzahl von Änderungen dauert länger. Der Service Level Agreement (SLA) gibt an, dass eine Änderung an einem Benutzer im SharePoint Onlineverzeichnis in der Benutzerprofilanwendung in 24 Stunden widergespiegelt wird. 
  
[Weitere Informationen zur Benutzerprofilsynchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

