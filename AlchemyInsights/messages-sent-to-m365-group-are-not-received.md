---
title: An eine Microsoft 365-Gruppe gesendete Nachrichten werden nicht von allen Mitgliedern empfangen
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976504"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>An eine Microsoft 365-Gruppe gesendete Nachrichten werden nicht von allen Mitgliedern empfangen

Stellen Sie sicher, dass alle Gruppenmitglieder den Empfang der E-Mails abonniert haben. Siehe [Folgen einer Gruppe in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Um den Nachrichtenstatus von Mitgliedern zu überprüfen, die Gruppen-E-Mails abonniert haben, führen Sie den folgenden Befehl in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) aus:

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Verwenden Sie den folgenden EXO PowerShell-Befehl, um alle Gruppenmitglieder so zu konfigurieren, dass sie E-Mails, die an die Microsoft 365-Gruppe gesendet werden, in ihrem Posteingang erhalten:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Beispiel:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`