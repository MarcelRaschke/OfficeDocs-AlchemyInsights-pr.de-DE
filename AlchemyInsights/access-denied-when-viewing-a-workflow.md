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
ms.openlocfilehash: e91e491c7ba0e240446bc0ca95e42864d192aed9
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61938968"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff verweigert beim Anzeigen eines Workflows

SharePoint 2013 workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.
  
 **Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**
  
 1. Zulassen, dass jeder die Mitglieder der SharePoint Gruppe sehen kann.
  
 2. Entfernen Sie die SharePoint Gruppe aus der Zeile "An" oder "CC" der E-Mail.
  
 3. Fügen Sie die Benutzer explizit zur Zeile "An" oder "CC" hinzu, wenn die Sichtbarkeit der Mitgliedschaft für SharePoint Gruppe nicht geändert werden kann.
  
Weitere Details finden Sie unter [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  