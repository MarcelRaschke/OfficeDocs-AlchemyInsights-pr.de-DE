---
title: Benutzern das Senden als Microsoft 365 Gruppe gestatten
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
- "9003200"
- "16400"
ms.date: 01/21/2022
ms.openlocfilehash: a38ce25a91c4a4fe982cc820c38982a455a01576
ms.sourcegitcommit: 5dcbecdebbf5042db0c86a12149ddd537d766c91
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2022
ms.locfileid: "62185298"
---
# <a name="allow-users-to-send-as-a-microsoft-365-group"></a>Benutzern das Senden als Microsoft 365 Gruppe gestatten

Verwenden Sie das Exchange Admin Center, oder stellen Sie eine Verbindung mit dem Exchange Online PowerShell-Befehl her, um einer Microsoft 365 Gruppe die Berechtigung "Senden als" zuzuweisen:

`Add-RecipientPermission <GroupName> -Trustee <MailboxName> -AccessRights SendAs`

Beispiel:

`Add-RecipientPermission MyGroup@contoso.onmicrosoft.com -Trustee Merry -AccessRights SendAs`

Weitere Informationen finden Sie unter [Zulassen, dass Mitglieder](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group) senden als oder senden im Namen einer Gruppe und Verbinden an Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).

Nachdem Berechtigungen zugewiesen wurden, kann der Benutzer E-Mails von der Gruppen-E-Mail-Adresse senden, indem er die folgenden Schritte ausführt:

1. Verfassen sie eine neue E-Mail.
2. Wählen Sie auf der Registerkarte **"Optionen"** unter **"Felder anzeigen"** die Option **"Von" aus.**
3. Geben Sie im Feld **"Von"** den Namen oder die E-Mail-Adresse der Gruppe ein, in deren Auftrag der Benutzer die Nachricht sendet.
