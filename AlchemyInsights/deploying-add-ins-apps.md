---
title: Bereitstellen von Add-Ins für Microsoft 365 Apps
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 991cc18aa01f2f9735dce60f543ac97d94ad7152
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63092926"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Bereitstellen von Add-Ins für Microsoft 365 Apps

Die zentrale Bereitstellung ist die empfohlene Methode zum Bereitstellen von Office-Add-Ins für Benutzer und Gruppen in Ihrer Organisation. Führen Sie die folgenden Schritte aus, um Add-Ins bereitzustellen:

**Hinweis:** Informationen zum Installieren von Add-Ins für Office als einzelner Benutzer finden Sie unter [Anzeigen, Verwalten und Installieren von Add-Ins in Office Programmen](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d). Stellen Sie außerdem sicher, dass der individuelle Erwerb von Office Store-Add-Ins aktiviert ist. Ausführliche Informationen finden Sie unter ["Verhindern von Add-In-Downloads durch Deaktivieren der Office Store auf allen Clients (außer Outlook)"](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. Stellen Sie sicher, dass Ihre Umgebung die Anforderungen für die Bereitstellung von Add-Ins mithilfe der zentralen Bereitstellung erfüllt. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Wechseln Sie im **Microsoft 365 Admin Center zu Einstellungen** >  **Integrated** **AppsGet-Apps** > , um Add-Ins bereitzustellen. 

Hinweise: 

- Integrierte Apps erfordern, dass der Administrator über globale Administrator- oder Exchange Administratorberechtigungen verfügt.

- Bei der Bereitstellung von Add-Ins für mehrere Benutzer wird empfohlen, Aufgaben mithilfe von Gruppen anstelle einzelner Benutzer durchzuführen. Ausführliche Informationen finden Sie unter ["Überlegungen beim Zuweisen eines Add-Ins zu Benutzern und Gruppen"](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins#considerations-when-assigning-an-add-in-to-users-and-groups).

- Die zentrale Bereitstellung unterstützt keine Benutzer in geschachtelten Gruppen oder Gruppen, die über übergeordnete Gruppen verfügen. Ausführliche Informationen finden Sie unter [Benutzer- und Gruppenzuweisungen](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins#user-and-group-assignments).

- Stellen Sie sicher, dass der Microsoft 365 App-Verwaltungsdienst (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') für Benutzer zur Anmeldung aktiviert ist. Ausführliche Informationen finden Sie unter [Konfigurieren von App-Eigenschaften](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Wenn Beim Bereitstellen von Add-Ins mithilfe integrierter Apps Probleme auftreten, versuchen Sie die Bereitstellung mithilfe von [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Weitere Informationen finden Sie unter:

[Bereitstellen von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
 [Verwalten von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
 [Verwenden der PowerShell-Cmdlets für die zentrale Bereitstellung zum Verwalten von Add-Ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
 [Veröffentlichen Office-Add-Ins mithilfe der zentralen Bereitstellung über das Microsoft 365 Admin Center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
 [Troubleshoot: Dem Benutzer werden keine Add-InsTroubleshoot-Benutzerfehler](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
 [mit Office-Add-Ins angezeigt](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)