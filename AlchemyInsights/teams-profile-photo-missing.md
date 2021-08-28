---
title: Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13260"
- "9008207"
ms.openlocfilehash: c0f8a6895299524e86f5519907b8d7c4bd9a9d42
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467384"
---
# <a name="teams-profile-photo-is-missing-or-cant-be-updated"></a>Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.

Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto in Microsoft Teams fehlt, überprüfen Sie Folgendes: 

- Benutzer freigegebener Postfächer können ihre Profilbilder nicht aktualisieren. Weitere Informationen finden Sie unter [Freigegebene Postfächer in Exchange Online](https://docs.microsoft.com/exchange/collaboration-exo/shared-mailboxes). 
- Das Postfach des Benutzers wurde in ein freigegebenes Postfach umgewandelt. Weitere Informationen finden Sie unter [Umwandeln eines Benutzerpostfachs in ein freigegebenes Postfach](https://docs.microsoft.com/microsoft-365/admin/email/convert-user-mailbox-to-shared-mailbox). 
- Der Benutzer verfügt über ein lokales Exchange-Postfach. Microsoft Teams berücksichtigt nur Exchange Online-Postfachrichtlinien für Outlook im Web (OWA), und diese Einstellungen werden für lokale Exchange-Benutzer nicht unterstützt. Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/exchange-teams-interact). 