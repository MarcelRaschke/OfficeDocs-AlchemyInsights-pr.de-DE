---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 13883a79a123833e3b5e424b7716dbd009618f4a
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62678587"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

Es gibt viele Möglichkeiten, den Zugriff auf SharePoint Online-/OneDrive-Dienste einzuschränken. Diese verschiedenen Methoden zur Zugriffseinschränkung werden unten beschrieben. 

**Berechtigungseinschränkung**

In SharePoint Online und OneDrive for Business beschränken wir den Zugriff auf Elemente wie Websites, Dateien und Ordner, indem wir nur den Gruppen/Personen Zugriff gewähren, die Zugriff haben sollten.

- [Anpassen von Berechtigungen für eine SharePoint Liste oder Bibliothek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Anpassen von SharePoint-Websiteberechtigungen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ändern der Berechtigungen für einen Unterordner](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Steuern des Zugriffs von nicht verwalteten Geräten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als SharePoint oder globaler Administrator können Sie den Zugriff auf SharePoint und OneDrive Inhalte von nicht verwalteten Geräten (die nicht mit Ad hybrid verbunden oder in Intune kompatibel sind) blockieren oder einschränken.

**Netzwerkstandorteinschränkung**

Als IT-Administrator können Sie den Zugriff auf SharePoint und OneDrive Ressourcen basierend auf definierten Netzwerkadressen steuern, denen Sie vertrauen. Dies wird auch als standortbasierte Richtlinie bezeichnet. Weitere Informationen finden Sie unter [Steuern des Zugriffs auf SharePoint Online- und OneDrive-Daten basierend auf dem Netzwerkstandort](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location).

**Einschränkung der Websitesperre** 

In SharePoint Online haben Sie die Möglichkeit, eine Websitesammlung zu sperren, sodass niemand Zugriff hat. Dies wird über PowerShell und die [SharePoint Online-Verwaltungsshell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps&preserve-view=true) mithilfe der [Set-SPOSite -LockState-Eigenschaft](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps&preserve-view=true) festgelegt.

**Benutzer am Erstellen von Websites oder Unterwebsites hindern**

Als SharePoint-Administrator oder globaler Administrator können Sie Ihren Benutzern erlauben, ihre eigenen SharePoint Websites zu erstellen und zu verwalten, zu bestimmen, welche Art von Websites sie erstellen können, und den Speicherort der Websites angeben. Weitere Informationen finden Sie unter [Verwalten der Websiteerstellung in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)
