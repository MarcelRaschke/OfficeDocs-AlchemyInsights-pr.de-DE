---
title: Inhalte werden in SharePoint-Suchergebnissen nicht angezeigt.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "5300017"
- "750"
ms.date: 04/21/2020
ms.openlocfilehash: 20a4c41a9837ad6734bd80c0e743b2e238d87039
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66379425"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Inhalte werden in SharePoint-Suchergebnissen nicht angezeigt.

Führen Sie die folgenden Schritte zur Problembehandlung aus, wenn erwarteter Inhalt nicht in den Suchergebnissen angezeigt wird:
  
1. Überprüfen Sie, ob die **Website** , die den erwarteten Inhalt enthält, so festgelegt ist, dass Inhalte in Suchergebnissen angezeigt werden. Führen Sie die Schritte unter [Anzeigen von Inhalten auf einer Website in Suchergebnissen](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results) aus.

2. Überprüfen Sie, ob die **Liste** oder **Bibliothek** , die den erwarteten Inhalt enthält, so festgelegt ist, dass Inhalte in Suchergebnissen angezeigt werden. Führen Sie die Schritte unter [Anzeigen von Inhalten aus Listen oder Bibliotheken in Suchergebnissen aus](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Stellen Sie sicher, dass das Seiten-, Dokument- oder benutzerdefinierte Seitenlayout als **Hauptversion** veröffentlicht wird. Schritt 3 in ["Suche" gibt nicht alle Ergebnisse in SharePoint Online zurück](https://go.microsoft.com/fwlink/?linkid=874525).

4. Stellen Sie sicher, dass der Benutzer **über Berechtigungen** zum Anzeigen des Inhalts verfügt. Führen Sie die Schritte unter [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels) aus.
    
5. Wenn das Suchschema durch Hinzufügen einer neuen verwalteten Eigenschaft, durch Bearbeiten einer verwalteten Eigenschaft oder durch Entfernen einer verwalteten Eigenschaft geändert wurde, ist das Anfordern einer Durchforstung und eines erneuten Indexes erforderlich. **Indizieren Sie** den Inhalt erneut, indem Sie die Schritte unter ["Manuelles Anfordern des Durchforstens und erneuten Indizierens einer Website, einer Bibliothek oder einer Liste" ausführen](https://docs.microsoft.com/sharepoint/crawl-site-content). Dies kann eine Weile dauern, warten Sie 24 Stunden, bevor Sie die Ergebnisse erneut überprüfen.

Weitere Informationen finden [Sie unter Aktivieren von Inhalten auf einer Website, um durchsuchbar zu sein](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
