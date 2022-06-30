---
title: Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9008207"
- "13260"
ms.date: 05/20/2022
ms.openlocfilehash: 3b9578fbe8cdf342f51590227391e0abb3d0b678
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66382320"
---
# <a name="teams-profile-photo-is-missing-or-cant-be-updated"></a>Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.

Profilfotos werden nicht sofort geändert. Mehrere Caches wirken sich auf das Foto aus, das ein Benutzer sieht.

Wenn ein Nutzer sein Foto ändert und das neue Foto überall sehen möchte, muss er den Cache seines Teams-Clients löschen oder 60 Tage warten (so lange dauert es, bis der Cache von Teams aktualisiert wird). Wenn ein anderer Benutzer das neue Benutzerfoto anzeigen möchte, muss er ebenfalls den eigenen Teams-Cache löschen oder 60 Tage warten. Weitere Informationen finden Sie unter [Löschen des Cache des Teams-Clients](https://docs.microsoft.com/microsoftteams/troubleshoot/teams-administration/clear-teams-cache).
 
Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto in Microsoft Teams fehlt, überprüfen Sie Folgendes:

- Benutzer freigegebener Postfächer können ihre Profilbilder nicht aktualisieren. Weitere Informationen finden Sie unter [Freigegebene Postfächer in Exchange Online](https://docs.microsoft.com/exchange/collaboration-exo/shared-mailboxes).
- Das Postfach des Benutzers wurde in ein freigegebenes Postfach umgewandelt. Weitere Informationen finden Sie unter [Umwandeln eines Benutzerpostfachs in ein freigegebenes Postfach](https://docs.microsoft.com/microsoft-365/admin/email/convert-user-mailbox-to-shared-mailbox).
- Der Benutzer verfügt über ein lokales Exchange-Postfach. Microsoft Teams berücksichtigt nur Exchange Online-Postfachrichtlinien für Outlook im Web (OWA), und diese Einstellungen werden für lokale Exchange-Benutzer nicht unterstützt. Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/exchange-teams-interact).