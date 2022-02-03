---
title: OneDrive for Business Web OneDrive leitet zu Delve
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: aeb9d288eed5d1d05e3c208a1cbe2186ac216f5c
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61867223"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Umgeleitet zu Delve, nachdem Sie auf OneDrive geklickt haben

Weitere Informationen finden Sie in unserem [ausführlichen Handbuch zur Problembehandlung.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Um dieses Problem zu beheben, muss der Administrator Benutzern das Recht erteilen, ihre Meine Websites-Website zu erstellen. Dies liegt daran, dass die OneDrive for Business Seite auf "Meine Websites" erstellt wird.

Führen Sie die folgenden Schritte aus, um dieses Recht zu gewähren:

1. Klicken Sie im SharePoint Admin Center auf **Benutzerprofile.**

2. Klicken Sie im Abschnitt **"Kontakte"** auf **"Benutzerberechtigungen verwalten".**

3. Fügen Sie Benutzer hinzu, die Berechtigungen zum Erstellen ihrer Website "Meine Websites" benötigen. Standardmäßig ist diese Einstellung auf **"Jeder"** mit Ausnahme externer Benutzer festgelegt.

4. Nachdem Sie den Benutzer, die Benutzer oder die Gruppe hinzugefügt haben, stellen Sie sicher, dass der hinzugefügte Benutzer, benutzer oder die Gruppe ausgewählt ist, scrollen Sie zum **Berechtigungsbereich,** und aktivieren Sie dann das Kontrollkästchen neben **"Persönliche Website erstellen" (erforderlich für persönlichen Speicher, Newsfeed und gefolgte Inhalte).**

5. Klicken Sie auf **"OK",** und lassen Sie den Benutzer zur OneDrive Seite navigieren, um die Website zu erstellen.
