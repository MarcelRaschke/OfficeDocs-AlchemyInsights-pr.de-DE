---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 26f1ea5156b4b153d5e804e0a09fd5b3295337d5
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61952804"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, nicht zugänglich oder für mehrere Benutzer nicht verfügbar

Wenn eine OneDrive oder SharePoint Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein vorübergehendes Dienstproblem auftreten. [Überprüfen Sie das Dienststatus-Dashboard.](https://portal.office.com/adminportal/home#/servicehealth)

**Hinzufügen und Lizenzieren des Benutzers**

Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 for Business Lizenzen zuweisen.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Zuweisen von Berechtigungen**

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und weiterhin eine Nachricht mit dem Zugriff verweigert wird, stellen Sie sicher, dass ihm die [entsprechende Berechtigungsstufe](https://docs.microsoft.com/sharepoint/understanding-permission-levels) zugewiesen wurde.

**Erwägen der Verwendung des Zugriffsanforderungsfeatures**

Die [Zugriffsanforderungsfunktion](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ermöglicht es Personen, Zugriff auf Inhalte anzufordern, für die sie derzeit nicht über die Berechtigung zum Anzeigen verfügen.

**Das Zulassen eines benutzerdefinierten Skripts kann Zutritt verweigerte Probleme verursachen.**

Es gibt bestimmte Szenarien, in denen das Feature *"Benutzerdefiniertes Skript zulassen"* möglicherweise einen Zugriff verweigert darstellt. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Besuchen Sie bitte ["Zulassen", oder verhindern Sie benutzerdefinierte Skripts.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

