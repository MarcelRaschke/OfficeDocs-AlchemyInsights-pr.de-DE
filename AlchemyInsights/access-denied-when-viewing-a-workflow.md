---
title: Zugriff beim Anzeigen eines Workflows verweigert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 1c4c61ee2d0268298a9e2792db9c2e921267f478
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66314859"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff beim Anzeigen eines Workflows verweigert

SharePoint 2013-Workflows, die versuchen, eine E-Mail an eine SharePoint-Gruppe zu senden, können mit der Fehlermeldung "Zugriff verweigert" fehlschlagen, wenn die Mitgliedschaft in der SharePoint-Gruppe nicht auf "Jeder" festgelegt ist.
  
 **Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**
  
 1. Jedem erlauben, die Mitglieder der SharePoint-Gruppe zu sehen.
  
 2. Entfernen Sie die SharePoint-Gruppe aus der Zeile "An" oder "CC" der E-Mail.
  
 3. Fügen Sie die Benutzer explizit der Zeile "An" oder "CC" hinzu, wenn die Sichtbarkeit der Mitgliedschaft für die SharePoint-Gruppe nicht geändert werden kann.
  
Weitere Details finden Sie unter [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  