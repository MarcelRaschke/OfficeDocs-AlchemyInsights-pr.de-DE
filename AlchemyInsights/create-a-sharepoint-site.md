---
title: Erstellen einer SharePoint-Website
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bbcfcc1fee42e63ddcd5b66298bfa601e07c52c0
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62670487"
---
# <a name="create-a-sharepoint-site"></a>Erstellen einer SharePoint-Website

Erstellen oder Verwalten von Websites über [aktive Websites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) im SharePoint Admin Center. Weitere Informationen finden Sie unter [Verwalten von Websites im neuen SharePoint Admin Center](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>Tipps:

- Sie **können** keine Website mit derselben URL einer vorhandenen Website erstellen. Wenn Sie eine Website gelöscht haben und die URL erneut verwenden möchten, ist es möglich, dass die gelöschte Website unter ["Gelöschte Websites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)" noch vorhanden ist. Die Website muss endgültig gelöscht werden, um die URL wieder zu verwenden. Informationen zum vollständigen Entfernen einer Website mit PowerShell finden Sie im Beispiel für das [Cmdlet "Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) ".
- Einige Benutzer können möglicherweise keine Website erstellen. [Siehe Verwalten der Websiteerstellung in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Es ist möglich, dass die Website beim **Erstellen** länger als erwartet hängen bleibt. Wenn seit dem ersten Auftreten dieses Problems mehr als 24 Stunden vergangen sind, melden Sie sich bitte ein Supportticket an. In vielen Fällen arbeiten wir bereits an einer Lösung. Bitte geben Sie uns mindestens 24 Stunden Zeit, um eine Lösung abzuschließen.
