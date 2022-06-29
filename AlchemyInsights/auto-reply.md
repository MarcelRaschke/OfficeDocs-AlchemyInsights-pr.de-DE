---
title: So konfigurieren Sie die automatische Antwort für alle an die Microsoft 365-Gruppe gesendeten E-Mails
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003200"
- "8586"
ms.date: 02/19/2021
ms.openlocfilehash: cc08ab0e8cd7c2ff032cfa09bde750e1eeb7136d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66299800"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>So konfigurieren Sie die automatische Antwort für alle an die Microsoft 365-Gruppe gesendeten E-Mails

**Stellen Sie eine Verbindung zur EXO PowerShell über das Administratorkonto des Mandanten her, und verwenden Sie folgenden Befehl**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**Hinweis**: Ändern Sie **groupmailbox** in einen Gruppennamen, für den Sie die automatische Antwort konfigurieren möchten.

