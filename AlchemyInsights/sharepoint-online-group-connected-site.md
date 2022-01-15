---
title: Hinzufügen einer Gruppe zu einer SharePoint Website
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 0ebd1a9ddd07f4b1cc08aa21144629cafebc2e70
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61965012"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Häufige Probleme beim Erstellen einer mit einer Gruppe verbundenen Website in SharePoint

1. Wenn Sie eine Gruppe und deren verbundene Website gelöscht haben und eine andere Website mit derselben URL erstellen möchten, müssen Sie die vorherige Website dauerhaft entfernen.

   - Herunterladen der [SPO-Verwaltungsshell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Weitere Informationen zu den ersten Schritten mit PowerShell finden Sie unter ["Erste Schritte mit SharePoint Online-Verwaltungsshell".](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Entfernen Sie die Website aus gelöschten Websites mithilfe des [Cmdlets "Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps&preserve-view=true) Powershell". PowerShell ist erforderlich, um Gruppenwebsites dauerhaft zu löschen.

1. If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Um das Problem zu beheben, löschen Sie die vorhandene Gruppe, wenn sie nicht mehr benötigt wird, oder erstellen Sie die Website mit einem anderen zugewiesenen Alias.

1. Es gibt verschiedene Möglichkeiten, moderne Gruppen mit SharePoint zu erstellen und zu verwenden.

   - Sie können vorhandene Websites mit einer Microsoft 365 Gruppe verbinden. Weitere Informationen finden Sie unter [Verbinden einer Microsoft 365-Gruppe mithilfe der SharePoint Benutzeroberfläche.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Um eine Microsoft 365 mit einer Gruppe verbundene Website zu erstellen, müssen Sie eine [Teamwebsite](https://admin.microsoft.com/sharepoint)erstellen.
