---
title: Bereitstellen von Add-Ins für Microsoft 365 Apps
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9005477"
- "11107"
ms.date: 04/30/2021
ms.openlocfilehash: 8c1c4dbe49c404943c438eab8c7d049b9ae4fde2
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66504787"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Bereitstellen von Add-Ins für Microsoft 365 Apps

Die zentrale Bereitstellung ist die empfohlene Methode für die Bereitstellung von Office-Add-Ins für Benutzer und Gruppen in Ihrer Organisation. Führen Sie die folgenden Schritte aus, um Add-Ins bereitzustellen:

**Hinweis:** Informationen zum Installieren von Add-Ins für Office als einzelner Benutzer finden Sie unter [Anzeigen, Verwalten und Installieren von Add-Ins in Office-Programmen](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d). Stellen Sie außerdem sicher, dass der individuelle Erwerb von Office Store-Add-Ins aktiviert ist. Ausführliche Informationen finden Sie unter ["Verhindern von Add-In-Downloads", indem Sie den Office Store für alle Clients (außer Outlook) deaktivieren](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. Stellen Sie sicher, dass Ihre Umgebung die Anforderungen für die Bereitstellung von Add-Ins mithilfe der zentralen Bereitstellung erfüllt. Ausführliche Informationen finden Sie unter ["Anforderungen"](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Wechseln **Sie zu "Integrierte****Apps** >  für Einstellungen" > **: Abrufen von Apps** in der Microsoft 365 Admin Center zum Bereitstellen von Add-Ins. 

Hinweise: 

- Integrierte Apps erfordern, dass der Administrator über globale Admin- oder Exchange Admin-Berechtigungen verfügt.

- Bei der Bereitstellung von Add-Ins für mehrere Benutzer wird empfohlen, Zuweisungen mithilfe von Gruppen anstelle einzelner Benutzer vorzunehmen. Ausführliche Informationen finden Sie [unter Überlegungen beim Zuweisen eines Add-Ins zu Benutzern und Gruppen](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins#considerations-when-assigning-an-add-in-to-users-and-groups).

- Die zentrale Bereitstellung unterstützt keine Benutzer in geschachtelten Gruppen oder Gruppen, die über übergeordnete Gruppen verfügen. Ausführliche Informationen finden Sie unter [Benutzer- und Gruppenzuweisungen](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins#user-and-group-assignments).

- Stellen Sie sicher, dass der Microsoft 365-App-Verwaltungsdienst (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') für die Anmeldung von Benutzern aktiviert ist. Ausführliche Informationen finden [Sie unter Konfigurieren von App-Eigenschaften](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Wenn Beim Bereitstellen von Add-Ins mithilfe integrierter Apps Probleme auftreten, versuchen Sie die Bereitstellung mithilfe von [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Weitere Informationen finden Sie unter:

[Bereitstellen von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
 [Verwalten von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
 [Verwenden der PowerShell-Cmdlets für die zentrale Bereitstellung zum Verwalten von Add-Ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
 [Veröffentlichen von Office-Add-Ins mithilfe der zentralen Bereitstellung über den Microsoft 365 Admin Center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
 [Troubleshoot: Benutzer sehen keine Add-Ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Beheben von Benutzerfehlern mit Office-Add-Ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)