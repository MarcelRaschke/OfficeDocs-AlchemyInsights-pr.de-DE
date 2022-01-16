---
title: Problembehandlung – Benutzer im Verzeichnis nicht gefunden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: e89979bba61f49da7f1b6f7d83eaaa592531d977
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61983213"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problembehandlung – Benutzer im Verzeichnis nicht gefunden

Wenn Benutzer die Fehlermeldung "Benutzer kann nicht gefunden werden" im Verzeichnis erhalten, versuchen Sie es erneut, wenn der Problemtyp "Benutzer" nicht im Verzeichnis ist.

Die folgenden Schritte können ausgeführt werden, um das Problem zu beheben.

- Stellen Sie sicher, dass das Konto, das die E-Mail-Einladung angenommen hat, dasselbe Konto ist, das später für die Anmeldung verwendet wird. Stellen Sie sicher, dass der Benutzer dasselbe Konto verwendet, um die Einladung zu akzeptieren und sich bei der Website anzumelden. 

Weitere Informationen finden Sie unter [Verwalten von Aliasen für Ihr Microsoft-Konto </a> zum Verwalten der Microsoft 365 Anmeldung.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Navigieren Sie zu allen Websites, auf denen der Benutzer den Fehler empfängt. 

Fügen Sie "/_layouts/15/people.aspx/membershipgroupid=0" (innerhalb der doppelten Anführungszeichen) am Ende der Website-URL hinzu. 

Beispiel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wählen Sie den Benutzer aus der Liste aus.

- Klicken Sie im Menüband auf **"Benutzerberechtigungen entfernen".** 
-  Fügen Sie den Benutzer zurück, und senden Sie die Einladung erneut an den Benutzer.

