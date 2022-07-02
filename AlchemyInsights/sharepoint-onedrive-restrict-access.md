---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: b35e0c95e0464d609f49795bdaff134fd3ce6928
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66598963"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

Es gibt viele Möglichkeiten, den Zugriff auf SharePoint Online/OneDrive-Dienste einzuschränken. Diese verschiedenen Zugriffseinschränkungsmethoden sind unten beschrieben. 

**Berechtigungseinschränkung**

In SharePoint Online und OneDrive for Business schränken wir den Zugriff auf Elemente wie Websites, Dateien und Ordner ein, indem nur diesen Gruppen/Personen Zugriff gewährt wird, die Zugriff haben sollen.

- [Anpassen von Berechtigungen für eine SharePoint-Liste oder -Bibliothek](https://support.microsoft.com/office/customize-permissions-for-a-sharepoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Anpassen von SharePoint-Websiteberechtigungen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ändern der Berechtigungen für einen Unterordner](https://support.microsoft.com/office/change-the-permissions-on-a-subfolder-5427bd7c-f20a-4f75-8cf2-5359dd45a1a6)

- [Steuern des Zugriffs von nicht verwalteten Geräten](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Als SharePoint- oder globaler Administrator können Sie den Zugriff auf SharePoint- und OneDrive-Inhalte von nicht verwalteten Geräten (solche, die nicht mit AD hybrid verbunden sind oder in Intune kompatibel sind) blockieren oder einschränken.

**Netzwerkstandorteinschränkung**

Als IT-Administrator können Sie den Zugriff auf SharePoint- und OneDrive-Ressourcen basierend auf definierten Netzwerkspeicherorten steuern, denen Sie vertrauen. Dies wird auch als standortbasierte Richtlinie bezeichnet. Weitere Informationen finden Sie unter [Steuern des Zugriffs auf SharePoint Online- und OneDrive-Daten basierend auf dem Netzwerkspeicherort](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location).

**Websitesperrungseinschränkung** 

In SharePoint Online haben Sie die Möglichkeit, eine Websitesammlung zu sperren, sodass niemand Zugriff hat. Dies wird über PowerShell und die [SharePoint Online-Verwaltungsshell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps&preserve-view=true) mithilfe der [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps&preserve-view=true) -LockState-Eigenschaft festgelegt.

**Benutzer am Erstellen von Websites oder Unterwebsites hindern**

Als SharePoint-Administrator oder globaler Administrator können Sie Es Ihren Benutzern ermöglichen, eigene SharePoint-Websites zu erstellen und zu verwalten, zu bestimmen, welche Art von Websites sie erstellen können, und den Speicherort der Websites angeben. Weitere Informationen finden Sie [unter Verwalten der Websiteerstellung in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)
