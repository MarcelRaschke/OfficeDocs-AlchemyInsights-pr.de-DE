---
title: Inhalt wird nicht in SharePoint Suchergebnissen angezeigt
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081609"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Inhalt wird nicht in SharePoint Suchergebnissen angezeigt

Führen Sie die folgenden Schritte zur Problembehandlung aus, wenn erwartete Inhalte nicht in Suchergebnissen angezeigt werden:
  
1. Überprüfen Sie, ob die **Website,** die den erwarteten Inhalt enthält, so festgelegt ist, dass Inhalte in Suchergebnissen angezeigt werden können. Führen Sie die Schritte unter [Anzeigen von Inhalten auf einer Website in Suchergebnissen](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)aus.

2. Überprüfen Sie, ob die **Liste** oder **Bibliothek,** die den erwarteten Inhalt enthält, so festgelegt ist, dass Inhalte in Suchergebnissen angezeigt werden können. Führen Sie die Schritte unter [Anzeigen von Inhalten aus Listen oder Bibliotheken in Suchergebnissen aus.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Stellen Sie sicher, dass die Seite, das Dokument oder das benutzerdefinierte Seitenlayout als Hauptversion veröffentlicht **wurde.** Schritt 3 in [Suche gibt nicht alle Ergebnisse in SharePoint Online zurück.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Stellen Sie sicher, dass der Benutzer **über Berechtigungen** zum Anzeigen des Inhalts verfügt. Führen Sie die Schritte unter [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)aus.
    
5. Wenn das Suchschema durch Hinzufügen einer neuen verwalteten Eigenschaft, Bearbeiten einer verwalteten Eigenschaft oder Entfernen einer verwalteten Eigenschaft geändert wurde, ist das Anfordern einer Durchforstung und eines erneuten Indizierens erforderlich. Führen Sie die Schritte in ["Manuelles Durchforsten und erneutes Indizieren einer Website, bibliothek oder Liste" durch,](https://docs.microsoft.com/sharepoint/crawl-site-content)um den Inhalt neu zu **indizieren.** Dies kann eine Weile dauern, warten Sie 24 Stunden, bevor Sie die Ergebnisse erneut überprüfen.

Weitere Informationen finden Sie unter Aktivieren der [Durchsuchbarkeit von Inhalten auf einer Website.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
