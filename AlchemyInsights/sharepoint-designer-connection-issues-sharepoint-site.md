---
title: SharePoint Designer-Verbindungsprobleme
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 35f905f08543aeb0fc81fa7b5ea8b3d811d96c59
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61981102"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-Verbindungsprobleme 

Wenn SharePoint Designer Verbindungsprobleme mit SharePoint Websites hat, probieren Sie die folgenden allgemeinen Lösungen aus.

Schritt 1: Stellen Sie sicher, dass SharePoint Designer 2013 mit [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) und dem Update vom [2. August 2016 für SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)aktualisiert wird.



Schritt 2: Löschen sie die lokalen Cachedateien:

1. Schließen Sie SharePoint Designer 2013.

2. Entfernen Sie auf dem lokalen Computer alle Dateien, die sich in den folgenden Ordnern befinden.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Öffnen Sie SharePoint Designer 2013, und geben Sie das Konto erneut ein, um festzustellen, ob es funktioniert.

Schritt 3: [Aktivieren Sie die moderne Authentifizierung für Office 2013 auf Windows Geräten.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Schritt 4: Administratoren müssen **benutzerdefinierte Skripts** in den Einstellungen des SharePoint Admin Center zulassen, um die SharePoint Designer-Verbindung zuzulassen. Weitere Informationen finden Sie unter [Zulassen oder Verhindern von benutzerdefinierten Skripts.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


