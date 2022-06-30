---
title: SharePoint Designer-Verbindungsprobleme
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.openlocfilehash: 6d0122515cf554d6e3c4db9ec3b32abfbb5c27bf
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66280882"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-Verbindungsprobleme 

Wenn in SharePoint Designer Verbindungsprobleme mit SharePoint-Websites auftreten, probieren Sie die folgenden allgemeinen Lösungen aus.

Schritt 1: Überprüfen Sie, ob SharePoint Designer 2013 mit [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) und dem [Update vom 2. August 2016 für SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721) aktualisiert wurde.



Schritt 2: Löschen der lokalen Cachedateien:

1. Schließen Sie SharePoint Designer 2013.

2. Entfernen Sie auf dem lokalen Computer alle Dateien, die sich in den folgenden Ordnern befinden.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Öffnen Sie SharePoint Designer 2013, und geben Sie das Konto erneut ein, um festzustellen, ob es funktioniert.

Schritt 3: [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Schritt 4: Administratoren müssen **benutzerdefinierte Skripts** in den SharePoint Admin Center-Einstellungen zulassen, um die SharePoint Designer-Verbindung zuzulassen. Weitere Informationen finden Sie unter ["Zulassen oder Verhindern von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) ".


