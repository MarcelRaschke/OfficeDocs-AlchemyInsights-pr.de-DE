---
title: Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: 66355290a6babb4d53cae561fb972eeba4ed875c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62750375"
---
# <a name="teams-profile-photo-is-missing-or-cant-be-updated"></a>Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.

Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto in Microsoft Teams fehlt, überprüfen Sie Folgendes: 

- Benutzer freigegebener Postfächer können ihre Profilbilder nicht aktualisieren. Weitere Informationen finden Sie unter [Freigegebene Postfächer in Exchange Online](https://docs.microsoft.com/exchange/collaboration-exo/shared-mailboxes). 
- Das Postfach des Benutzers wurde in ein freigegebenes Postfach umgewandelt. Weitere Informationen finden Sie unter [Umwandeln eines Benutzerpostfachs in ein freigegebenes Postfach](https://docs.microsoft.com/microsoft-365/admin/email/convert-user-mailbox-to-shared-mailbox). 
- Der Benutzer verfügt über ein lokales Exchange-Postfach. Microsoft Teams berücksichtigt nur Exchange Online-Postfachrichtlinien für Outlook im Web (OWA), und diese Einstellungen werden für lokale Exchange-Benutzer nicht unterstützt. Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/exchange-teams-interact). 