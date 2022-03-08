---
title: Zugriff auf SharePoint oder OneDrive Admin Center nicht möglich
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 80369bd9f38b357361b404e565b75b35c9b0f419
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63082306"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Zugriff auf SharePoint oder OneDrive Admin Center nicht möglich

- Wenn Ihre SharePoint- oder OneDrive-Admin Center-Website nicht zugänglich oder nicht verfügbar ist, kann es ein vorübergehendes Dienstproblem geben, bei dem Benutzer beim Zugriff auf SharePoint-Websites oder OneDrive-Inhalte zeitweilige Verzögerungen oder Navigationsfehler feststellen. Prüfen Sie das [Dienststatus-Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth), ob Ihre Organisation betroffen ist.

- Globalen Administratoren und SharePoint-Administratoren muss eine SharePoint-Lizenz zugewiesen werden. Neu erstellte Konten, denen nur eine SharePoint-Lizenz oder nur die Administratorrolle zugewiesen wird, können Probleme beim Zugriff auf SharePoint feststellen, z. B. "Zugriff verweigert" oder "Benutzer nicht gefunden". Warten Sie mindestens 24 Stunden, bis die Synchronisierung zwischen unseren Systemen abgeschlossen ist. Wir verstehen, dass Ihnen 24 Stunden lang vorkommen mag. In vielen Fällen arbeiten wir bereits an einer Lösung.

- Benutzern von Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) kann der Zugriff verweigert werden, wenn das Zeitfenster für den erlaubten Zugriff sehr klein ist, siehe [Zugriff auf PIM-Konten verweigert](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).