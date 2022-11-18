---
title: Problembehandlung bei Nachrichten mit verweigertem Zugriff
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 6c82a5e4da2857cf54ab9c529c6f5e58aef75912
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66590467"
---
# <a name="troubleshoot-access-denied-messages"></a>Problembehandlung bei Nachrichten mit verweigertem Zugriff

Wenn Sie beim Versuch, eine SharePoint Online-Website zu durchsuchen, eine Meldung über den Verweigerten Zugriff erhalten, lesen Sie die folgenden Artikel.

**Hinzufügen und Lizenzieren des Benutzers**

Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 Business Lizenzen zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**Berechtigungen zuweisen**

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und dennoch eine Meldung über den Verweigerten Zugriff angezeigt wird, stellen Sie sicher, dass ihm die [entsprechende Berechtigungsstufe zugewiesen ist](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

**Erwägen Sie die Verwendung des Zugriffsanforderungsfeatures**

Das [Feature "Zugriffsanforderung](https://support.microsoft.com/office/set-up-and-manage-access-requests-94b26e0b-2822-49d4-929a-8455698654b3) " ermöglicht Es Personen, Zugriff auf Inhalte anzufordern, für die sie derzeit nicht über die Berechtigung zum Anzeigen verfügen. 

**Das Zulassen benutzerdefinierter Skripts kann zu Problemen mit dem Verweigerten Zugriff führen.**

Es gibt bestimmte Szenarien, in denen das Feature "Benutzerdefiniertes Skript zulassen" möglicherweise einen verweigerten Zugriff darstellt. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Besuchen Sie , [erlauben oder verhindern Sie benutzerdefinierte Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Hinweis: Wenn eine OneDrive- oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, liegt möglicherweise ein temporäres Dienstproblem vor. [Überprüfen Sie das Dienstintegritätsdashboard](https://portal.office.com/adminportal/home#/servicehealth).


  

