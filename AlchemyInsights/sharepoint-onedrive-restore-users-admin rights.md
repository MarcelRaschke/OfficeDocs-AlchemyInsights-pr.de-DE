---
title: Problembehandlung bei Zugriff verweigerten Nachrichten auf OneDrive for Business Websites
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d1d50f924cae64a72e428de8d22c09c43ed9aac
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61962691"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problembehandlung bei Zugriff verweigerten Nachrichten auf OneDrive for Business Websites

Dieses Problem tritt am häufigsten auf, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen PUID-Werts (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, hat der Benutzer eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory-Organisationseinheit (OU). Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere OU verschoben und mit SharePoint erneut synchronisiert werden, kann dieses Problem auftreten.

1. Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel [Wiederherstellen eines Benutzers in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)wiederherstellen.
2. Wenn Sie den ursprünglichen Benutzer nicht wiederherstellen können, sollten Sie den alten Benutzer mit den folgenden Schritten aus der OneDrive Website entfernen. [Entfernen Sie einen Benutzer aus der Benutzerinformationsliste.]() 
3. Danach können Sie überprüfen, ob der Benutzer über Administratorrechte für die OneDrive Website verfügt, indem Sie die Schritte zum Hinzufügen von [Administratoren für die OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Weitere Informationen zu Berechtigungsstufen finden Sie im Artikel ["Grundlegendes zu Berechtigungsstufen in SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
