---
title: Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: e247c0e5f5c6771964178438c62160b153741053
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62715057"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail

Der Absender einer E-Mail-Nachricht an eine Microsoft 365-Gruppe empfängt standardmäßig keine Kopie der Nachricht in seinem Posteingang, auch er ein Mitglied der Gruppe ist.

Mit diesem EXO PowerShell-Befehl können Sie dem Absender das Empfangen einer Kopie jeder E-Mail erlauben, die er an die Microsoft 365-Gruppe sendet:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

So aktivieren Sie die Einstellung für alle Postfächer gleichzeitig:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Hinweis** Änderungen an dieser Einstellung dauern bis zu einer Stunde, bis sie wirksam werden.