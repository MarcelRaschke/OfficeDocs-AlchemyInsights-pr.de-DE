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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d1fd9ff3c1be7dc15d6d67441f04c998991a40a5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63151014"
---
# <a name="turn-on-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Um die Postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, führen Sie die folgenden Cmdlets über Remote PowerShell aus:

- **Einzelner Benutzer**: Set-Mailbox -Identity "Jane Maustaste" -AuditEnabled $true
- **Organisation**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Weitere Informationen finden Sie unter [Verwalten der Postfachüberwachung](https://go.microsoft.com/fwlink/?linkid=2103668).