---
title: So konfigurieren Sie die automatische Antwort für alle an die Microsoft 365-Gruppe gesendeten E-Mails
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 8f79ba7f4c00199bb663a6dfa735128576dc2420
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62594447"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>So konfigurieren Sie die automatische Antwort für alle an die Microsoft 365-Gruppe gesendeten E-Mails

**Stellen Sie eine Verbindung zur EXO PowerShell über das Administratorkonto des Mandanten her, und verwenden Sie folgenden Befehl**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**Hinweis**: Ändern Sie **groupmailbox** in einen Gruppennamen, für den Sie die automatische Antwort konfigurieren möchten.

