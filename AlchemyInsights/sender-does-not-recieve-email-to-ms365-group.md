---
title: Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958296"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail

Der Absender einer E-Mail-Nachricht an eine Microsoft 365-Gruppe empfängt standardmäßig keine Kopie der Nachricht in seinem Posteingang, auch er ein Mitglied der Gruppe ist.

Mit diesem EXO PowerShell-Befehl können Sie dem Absender das Empfangen einer Kopie jeder E-Mail erlauben, die er an die Microsoft 365-Gruppe sendet:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

So aktivieren Sie die Einstellung für alle Postfächer gleichzeitig:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Hinweis** Änderungen an dieser Einstellung dauern bis zu einer Stunde, bis sie wirksam werden.