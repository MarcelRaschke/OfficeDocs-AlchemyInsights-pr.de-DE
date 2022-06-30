---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 5def7c004bbe5c33e9ccf2647f1e4237f140fd78
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66373215"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive Slow, Nicht zugänglich oder für mehrere Benutzer nicht verfügbar

Wenn eine OneDrive- oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, liegt möglicherweise ein temporäres Dienstproblem vor. [Überprüfen Sie das Dienstintegritätsdashboard](https://portal.office.com/adminportal/home#/servicehealth).

**Hinzufügen und Lizenzieren des Benutzers**

Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 Business Lizenzen zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Berechtigungen zuweisen**

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und dennoch eine Meldung über den Verweigerten Zugriff angezeigt wird, stellen Sie sicher, dass ihm die [entsprechende Berechtigungsstufe](https://docs.microsoft.com/sharepoint/understanding-permission-levels) zugewiesen ist.

**Erwägen Sie die Verwendung des Zugriffsanforderungsfeatures**

Das [Feature "Zugriffsanforderung](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) " ermöglicht Es Personen, Zugriff auf Inhalte anzufordern, für die sie derzeit nicht über die Berechtigung zum Anzeigen verfügen.

**Das Zulassen benutzerdefinierter Skripts kann zu Problemen mit dem Verweigerten Zugriff führen.**

Es gibt bestimmte Szenarien, in denen das Feature *"Benutzerdefiniertes Skript zulassen* " möglicherweise einen verweigerten Zugriff darstellt. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Besuchen Sie ["Benutzerdefiniertes Skript zulassen oder verhindern"](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

