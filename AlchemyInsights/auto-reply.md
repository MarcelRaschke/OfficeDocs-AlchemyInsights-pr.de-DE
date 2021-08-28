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
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331530"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>So konfigurieren Sie die automatische Antwort für alle an die Microsoft 365-Gruppe gesendeten E-Mails

**Stellen Sie eine Verbindung zur EXO PowerShell über das Administratorkonto des Mandanten her, und verwenden Sie folgenden Befehl**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**Hinweis**: Ändern Sie **groupmailbox** in einen Gruppennamen, für den Sie die automatische Antwort konfigurieren möchten.

