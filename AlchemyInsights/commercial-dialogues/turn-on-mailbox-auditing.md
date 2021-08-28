---
title: Aktivieren der Postfachüberwachung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058037"
---
# <a name="turn-on-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Um die Postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, führen Sie die folgenden Cmdlets über Remote PowerShell aus:

- **Einzelner Benutzer**: Set-Mailbox -Identity "Jane Maustaste" -AuditEnabled $true
- **Organisation**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Weitere Informationen finden Sie unter [Verwalten der Postfachüberwachung.](https://go.microsoft.com/fwlink/?linkid=2103668)