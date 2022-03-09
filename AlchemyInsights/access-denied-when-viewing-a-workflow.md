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
ms.localizationpriority: medium
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: d1642a53cd6f9fa3fcfcaf829f4fb55e91987886
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63288773"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Zugriff verweigert beim Anzeigen eines Workflows

SharePoint 2013-Workflows, die versuchen, eine E-Mail an eine SharePoint-Gruppe zu senden, können mit der Fehlermeldung "Zugriff verweigert" fehlschlagen, wenn die Mitgliedschaft der SharePoint-Gruppe nicht auf "Jeder" festgelegt ist.
  
 **Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:**
  
 1. Zulassen, dass jeder die Mitglieder der SharePoint-Gruppe sehen kann.
  
 2. Entfernen Sie die SharePoint-Gruppe aus der Zeile "An" oder "CC" der E-Mail.
  
 3. Fügen Sie die Benutzer explizit zur Zeile "An" oder "CC" hinzu, wenn die Sichtbarkeit der Mitgliedschaft für die SharePoint-Gruppe nicht geändert werden kann.
  
Weitere Details finden Sie unter [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  