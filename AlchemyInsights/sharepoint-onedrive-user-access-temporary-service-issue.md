---
title: Leistungsprobleme SharePoint oder OneDrive
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
ms.openlocfilehash: ca3f8787237f8f6bd82e90c6bf3fa89929f74a3c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62707101"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, nicht zugänglich oder für mehrere Benutzer nicht verfügbar

Wenn eine OneDrive oder SharePoint Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein vorübergehendes Dienstproblem auftreten. [Überprüfen Sie das Dienststatus-Dashboard](https://portal.office.com/adminportal/home#/servicehealth).

**Hinzufügen und Lizenzieren des Benutzers**

Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 business Lizenzen zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Zuweisen von Berechtigungen**

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und weiterhin eine Nachricht mit dem Zugriff verweigert wird, stellen Sie sicher, dass ihm die [entsprechende Berechtigungsstufe](https://docs.microsoft.com/sharepoint/understanding-permission-levels) zugewiesen wurde.

**Erwägen der Verwendung des Zugriffsanforderungsfeatures**

Die [Zugriffsanforderungsfunktion](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ermöglicht es Personen, Zugriff auf Inhalte anzufordern, für die sie derzeit nicht über die Berechtigung zum Anzeigen verfügen.

**Das Zulassen eines benutzerdefinierten Skripts kann Zutritt verweigerte Probleme verursachen.**

Es gibt bestimmte Szenarien, in denen das Feature " *Benutzerdefiniertes Skript zulassen* " möglicherweise einen Zugriff verweigert darstellt. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Besuchen Sie bitte ["Zulassen" oder "Benutzerdefiniertes Skript verhindern](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)".

