---
title: Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003200"
ms.date: 08/20/2020
ms.openlocfilehash: 40fd2726595e928d11230a5edea83334eadad6ab
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66398955"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Absender empfängt keine an eine Microsoft 365-Gruppe gesendete E-Mail

Der Absender einer E-Mail-Nachricht an eine Microsoft 365-Gruppe empfängt standardmäßig keine Kopie der Nachricht in seinem Posteingang, auch er ein Mitglied der Gruppe ist.

Mit diesem EXO PowerShell-Befehl können Sie dem Absender das Empfangen einer Kopie jeder E-Mail erlauben, die er an die Microsoft 365-Gruppe sendet:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

So aktivieren Sie die Einstellung für alle Postfächer gleichzeitig:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Hinweis** Änderungen an dieser Einstellung dauern bis zu einer Stunde, bis sie wirksam werden.