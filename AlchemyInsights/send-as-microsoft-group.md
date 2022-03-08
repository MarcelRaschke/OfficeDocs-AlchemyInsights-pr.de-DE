---
title: Benutzern das Senden als Microsoft 365 Gruppe gestatten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "16400"
ms.date: 01/21/2022
ms.openlocfilehash: 0e947984667cbef57d8c888cd21abdfc2af7ade2
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63222009"
---
# <a name="allow-users-to-send-as-a-microsoft-365-group"></a>Benutzern das Senden als Microsoft 365 Gruppe gestatten

Verwenden Sie das Exchange Admin Center, oder stellen Sie eine Verbindung mit dem Exchange Online PowerShell-Befehl her, um einer Microsoft 365 Gruppe die Berechtigung "Senden als" zuzuweisen:

`Add-RecipientPermission <GroupName> -Trustee <MailboxName> -AccessRights SendAs`

Beispiel:

`Add-RecipientPermission MyGroup@contoso.onmicrosoft.com -Trustee Merry -AccessRights SendAs`

Weitere Informationen finden Sie unter [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group) and [Verbinden to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).

Nachdem Berechtigungen zugewiesen wurden, kann der Benutzer E-Mails von der Gruppen-E-Mail-Adresse senden, indem er die folgenden Schritte ausführt:

1. Verfassen sie eine neue E-Mail.
2. Wählen Sie auf der Registerkarte **"Optionen** " unter **"Felder anzeigen**" **die Option "Von" aus**.
3. Geben Sie im Feld **"Von** " den Namen oder die E-Mail-Adresse der Gruppe ein, in deren Auftrag der Benutzer die Nachricht sendet.
