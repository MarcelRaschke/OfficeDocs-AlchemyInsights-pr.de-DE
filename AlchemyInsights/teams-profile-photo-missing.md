---
title: Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.
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
- "13260"
- "9008207"
ms.date: 05/20/2022
ms.openlocfilehash: d1564a5539856ac2188998fc579baae6e346dd55
ms.sourcegitcommit: bc551e8b105d0a79f09a690722a36130fdd69173
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/20/2022
ms.locfileid: "65620636"
---
# <a name="teams-profile-photo-is-missing-or-cant-be-updated"></a>Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.

Profilfotos werden nicht sofort geändert. Mehrere Caches wirken sich auf das Foto aus, das ein Benutzer sieht.

Wenn ein Nutzer sein Foto ändert und das neue Foto überall sehen möchte, muss er den Cache seines Teams-Clients löschen oder 60 Tage warten (so lange dauert es, bis der Cache von Teams aktualisiert wird). Wenn ein anderer Benutzer das neue Benutzerfoto anzeigen möchte, muss er ebenfalls den eigenen Teams-Cache löschen oder 60 Tage warten. Weitere Informationen finden Sie unter [Löschen des Cache des Teams-Clients](https://docs.microsoft.com/microsoftteams/troubleshoot/teams-administration/clear-teams-cache).
 
Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto in Microsoft Teams fehlt, überprüfen Sie Folgendes:

- Benutzer freigegebener Postfächer können ihre Profilbilder nicht aktualisieren. Weitere Informationen finden Sie unter [Freigegebene Postfächer in Exchange Online](https://docs.microsoft.com/exchange/collaboration-exo/shared-mailboxes).
- Das Postfach des Benutzers wurde in ein freigegebenes Postfach umgewandelt. Weitere Informationen finden Sie unter [Umwandeln eines Benutzerpostfachs in ein freigegebenes Postfach](https://docs.microsoft.com/microsoft-365/admin/email/convert-user-mailbox-to-shared-mailbox).
- Der Benutzer verfügt über ein lokales Exchange-Postfach. Microsoft Teams berücksichtigt nur Exchange Online-Postfachrichtlinien für Outlook im Web (OWA), und diese Einstellungen werden für lokale Exchange-Benutzer nicht unterstützt. Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/exchange-teams-interact).