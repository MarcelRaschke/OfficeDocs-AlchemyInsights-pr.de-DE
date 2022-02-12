---
title: Senden als Microsoft 365-Gruppe
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: abe3319f175ea19da09825cf743c6630f8b8df40
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62632218"
---
# <a name="send-as-microsoft-365-group"></a>Senden als Microsoft 365-Gruppe

Sie können "Senden als"-Berechtigungen zuweisen, um bestimmten Benutzern das Senden von Nachrichten als Microsoft 365-Gruppe zu erlauben:  

1. Stellen Sie eine Verbindung mit Exchange Online PowerShell her.  

2. Führen Sie den folgenden Befehl aus:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Weitere Informationen finden Sie unter [Zulassen, dass Mitglieder mit "Senden als" oder "Senden im Auftrag von" E-Mails für eine Gruppe senden](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group).