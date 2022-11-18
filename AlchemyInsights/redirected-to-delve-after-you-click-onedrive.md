---
title: OneDrive for Business Web OneDrive leitet zu Delve um
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "900072"
- "1870"
ms.openlocfilehash: 992a3e6f995db990fc876289aa38e97e4d639a01
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66264988"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Umgeleitet nach Delve, nachdem Sie auf OneDrive geklickt haben

Weitere Informationen finden Sie in unserem detaillierten [Handbuch zur Problembehandlung](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Um dieses Problem zu beheben, muss der Administrator Benutzern das Recht erteilen, ihre Website "Meine Websites" zu erstellen. Dies liegt daran, dass die OneDrive for Business Seite auf "Meine Websites" erstellt wird.

Führen Sie die folgenden Schritte aus, um dieses Recht zu gewähren:

1. Klicken Sie im SharePoint Admin Center auf **Benutzerprofile**.

2. Klicken Sie im Abschnitt **"Personen** " auf **"Benutzerberechtigungen verwalten"**.

3. Fügen Sie Benutzer hinzu, die Berechtigungen zum Erstellen ihrer Website "Meine Websites" benötigen. Standardmäßig ist diese Einstellung auf **"Jeder außer externen Benutzern**" festgelegt.

4. Nachdem Sie den Benutzer, die Benutzer oder die Gruppe hinzugefügt haben, stellen Sie sicher, dass der hinzugefügte Benutzer, die Benutzer oder die Gruppe ausgewählt ist, scrollen Sie zum **Abschnitt "Berechtigungen**", und aktivieren Sie dann das Kontrollkästchen neben **"Persönliche Website erstellen" (erforderlich für persönlichen Speicher, Newsfeed und gefolgte Inhalte).**

5. Klicken Sie auf **"OK**", und lassen Sie den Benutzer zur OneDrive-Seite navigieren, um die Website zu erstellen.
