---
title: Problembehandlung bei Zugriff verweigerten Nachrichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6a0b3c274e9bb77b6416d919e2ad53a03597d271
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62693289"
---
# <a name="troubleshoot-access-denied-messages"></a>Problembehandlung bei Zugriff verweigerten Nachrichten

Wenn Sie beim Versuch, eine Sharepoint Online-Website zu durchsuchen, eine Meldung erhalten, die den Zugriff verweigert, lesen Sie die folgenden Artikel.

**Hinzufügen und Lizenzieren des Benutzers**

Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 business Lizenzen zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**Zuweisen von Berechtigungen**

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und weiterhin eine Nachricht mit dem Zugriff verweigert wird, stellen Sie sicher, dass ihm die [entsprechende Berechtigungsstufe zugewiesen wurde](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

**Erwägen der Verwendung des Zugriffsanforderungsfeatures**

Die [Zugriffsanforderungsfunktion](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ermöglicht es Personen, Zugriff auf Inhalte anzufordern, für die sie derzeit nicht über die Berechtigung zum Anzeigen verfügen. 

**Das Zulassen eines benutzerdefinierten Skripts kann Zutritt verweigerte Probleme verursachen.**

Es gibt bestimmte Szenarien, in denen das Feature "Benutzerdefiniertes Skript zulassen" möglicherweise den Zugriff verweigert. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Besuchen Sie [bitte benutzerdefinierte Skripts, um sie zuzulassen oder zu verhindern](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

Hinweis: Wenn eine OneDrive oder SharePoint Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein vorübergehendes Dienstproblem auftreten. [Überprüfen Sie das Dienststatus-Dashboard](https://portal.office.com/adminportal/home#/servicehealth).


  

