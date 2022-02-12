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
ms.openlocfilehash: d0222e7a305338c3cdc3ce8a3534109b32e3cc2c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62616252"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problembehandlung bei Zugriff verweigerten Nachrichten in Sharepoint/OneDrive Admin Center

Wenn Sie beim Versuch, zu einem Sharepoint/OneDrive Admin Center zu navigieren, eine Meldung erhalten, dass der Zugriff verweigert wird, stellen Sie sicher, dass Sie [dem Benutzer eine Lizenz zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Wenn der Benutzer über eine Lizenz verfügt, sollten Sie auch sicherstellen, dass ihm [eine Administratorrolle zugewiesen](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ist, die auf die Admin Center zugreifen kann.

Dieses Problem kann auch auftreten, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen PUID-Werts (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, hat der Benutzer eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory-Organisationseinheit (OU). Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere OU verschoben und mit SharePoint erneut synchronisiert werden, kann dieses Problem auftreten.

Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel "[Wiederherstellen eines Benutzers in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)" wiederherstellen.

Hinweis: Wenn ein OneDrive oder SharePoint Admin Center nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, liegt möglicherweise ein vorübergehendes Dienstproblem vor.  [Überprüfen Sie das Dienststatus-Dashboard](https://portal.office.com/adminportal/home#/servicehealth).


