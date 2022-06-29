---
title: Zulassen, dass Benutzer als Microsoft 365-Gruppe senden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003200"
- "16400"
ms.date: 01/21/2022
ms.openlocfilehash: 2b56a9d775d63ddb8e62d1d089e59ebf85eeda83
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66317019"
---
# <a name="allow-users-to-send-as-a-microsoft-365-group"></a>Zulassen, dass Benutzer als Microsoft 365-Gruppe senden

Verwenden Sie das Exchange Admin Center, oder stellen Sie eine Verbindung mit dem Exchange Online PowerShell-Befehl her, um einer Microsoft 365-Gruppe die Berechtigung "Senden als" zuzuweisen:

`Add-RecipientPermission <GroupName> -Trustee <MailboxName> -AccessRights SendAs`

Beispiel:

`Add-RecipientPermission MyGroup@contoso.onmicrosoft.com -Trustee Merry -AccessRights SendAs`

Weitere Informationen finden Sie unter ["Mitgliedern das Senden als oder Senden im Auftrag einer Gruppe erlauben](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group)" und "[Herstellen einer Verbindung mit Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)".

Nachdem Berechtigungen zugewiesen wurden, kann der Benutzer E-Mails über die Gruppen-E-Mail-Adresse senden, indem er die folgenden Schritte ausführt:

1. Verfassen sie eine neue E-Mail.
2. Wählen Sie auf der Registerkarte **"Optionen** " unter **"Felder anzeigen"** die Option **"Von" aus**.
3. Geben Sie im Feld **"Von** " den Namen oder die E-Mail-Adresse der Gruppe ein, in deren Namen der Benutzer die Nachricht sendet.
