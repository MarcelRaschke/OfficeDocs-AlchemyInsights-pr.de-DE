---
title: Hinzufügen einer Gruppe zu einer SharePoint-Website
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "5200004"
- "5766"
ms.openlocfilehash: 66f01de589d4a37ca1bfc507153fcc31f94071fb
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66593419"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Häufige Probleme beim Erstellen einer mit einer Gruppe verbundenen Website in SharePoint

1. Wenn Sie eine Gruppe und ihre verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website endgültig entfernen.

   - [Herunterladen der SPO-Verwaltungsshell](https://support.microsoft.com/office/introduction-to-the-sharepoint-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Weitere Informationen zu den ersten Schritten mit PowerShell finden [Sie unter "Erste Schritte mit der SharePoint Online-Verwaltungsshell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)".
   - Entfernen Sie die Website mithilfe des Cmdlets [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps&preserve-view=true) Powershell von gelöschten Websites. Powershell ist erforderlich, um Gruppenwebsites dauerhaft zu löschen.

1. Wenn Sie eine mit einer Gruppe verbundene Website erstellen und eine Warnung erhalten: **Eine andere Gruppe mit demselben Alias ist bereits vorhanden**, überprüfen Sie die vorhandenen Gruppen aus der [Microsoft 365 Admin Center](https://admin.microsoft.com/adminportal/home?ref=groups). Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen Alias.

1. Es gibt verschiedene Möglichkeiten, moderne Gruppen mit SharePoint zu erstellen und zu verwenden.

   - Sie können vorhandene Websites mit einer Microsoft 365-Gruppe verbinden. Weitere Informationen finden Sie unter [Verbinden einer Microsoft 365-Gruppe mithilfe der SharePoint-Benutzeroberfläche](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Um eine mit Microsoft 365-Gruppen verbundene Website zu erstellen, müssen Sie eine [Teamwebsite](https://admin.microsoft.com/sharepoint) erstellen.
