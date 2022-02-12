---
title: Zugriff verweigert beim Anzeigen eines Workflows
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: fe6e4802c68e94015928a6f79fa6ee2add312d59
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62565435"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff verweigert beim Anzeigen eines Workflows

SharePoint 2013 workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.
  
 **Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**
  
 1. Zulassen, dass jeder die Mitglieder der SharePoint Gruppe sehen kann.
  
 2. Entfernen Sie die SharePoint Gruppe aus der Zeile "An" oder "CC" der E-Mail.
  
 3. Fügen Sie die Benutzer explizit zur Zeile "An" oder "CC" hinzu, wenn die Sichtbarkeit der Mitgliedschaft für SharePoint Gruppe nicht geändert werden kann.
  
Weitere Informationen finden Sie unter [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  