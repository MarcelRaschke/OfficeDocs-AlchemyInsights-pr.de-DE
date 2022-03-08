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
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "13260"
- "9008207"
ms.openlocfilehash: 6c20321b19f78386b4d6d614229e30b25bec6ba5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63084178"
---
# <a name="teams-profile-photo-is-missing-or-cant-be-updated"></a>Das Teams-Profilfoto fehlt oder kann nicht aktualisiert werden.

Wenn für mindestens eine Person in Ihrer Organisation das Profilfoto in Microsoft Teams fehlt, überprüfen Sie Folgendes: 

- Benutzer freigegebener Postfächer können ihre Profilbilder nicht aktualisieren. Weitere Informationen finden Sie unter [Freigegebene Postfächer in Exchange Online](https://docs.microsoft.com/exchange/collaboration-exo/shared-mailboxes). 
- Das Postfach des Benutzers wurde in ein freigegebenes Postfach umgewandelt. Weitere Informationen finden Sie unter [Umwandeln eines Benutzerpostfachs in ein freigegebenes Postfach](https://docs.microsoft.com/microsoft-365/admin/email/convert-user-mailbox-to-shared-mailbox). 
- Der Benutzer verfügt über ein lokales Exchange-Postfach. Microsoft Teams berücksichtigt nur Exchange Online-Postfachrichtlinien für Outlook im Web (OWA), und diese Einstellungen werden für lokale Exchange-Benutzer nicht unterstützt. Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/exchange-teams-interact). 