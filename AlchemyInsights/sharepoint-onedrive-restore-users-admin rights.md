---
title: Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive for Business Websites
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.openlocfilehash: 56cc22d8837adbec75d7a733aae62aa8f83f7d48
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66425784"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive for Business Websites

Dieses Problem tritt am häufigsten auf, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen PUID-Werts (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder sein OneDrive zuzugreifen, hat der Benutzer eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory-Organisationseinheit (OU). Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere ORGANISATIONSeinheit verschoben und erneut mit SharePoint synchronisiert werden, kann dieses Problem auftreten.

1. Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel [Wiederherstellen eines Benutzers in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user) wiederherstellen.
2. Wenn Sie den ursprünglichen Benutzer nicht wiederherstellen können, sollten Sie den alten Benutzer mithilfe dieser Schritte von der OneDrive-Website entfernen. [Entfernen Sie einen Benutzer aus der Benutzerinformationenliste](). 
3. Anschließend können Sie überprüfen, ob der Benutzer über Administratorrechte für die OneDrive-Website verfügt, indem Sie die Schritte zum [Hinzufügen von Administratoren für oneDrive eines Benutzers](https://docs.microsoft.com/sharepoint/manage-user-profiles) ausführen.

Weitere Informationen zu Berechtigungsstufen finden Sie im Artikel ["Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)".
