---
title: Aktivieren der Postfachüberwachung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100005"
- "7327"
ms.date: 02/26/2021
ms.openlocfilehash: 9473ecb7a0aac507078f491752c81de20da2fac7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66424264"
---
# <a name="turn-on-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Führen Sie die folgenden Cmdlets von Remote PowerShell aus, um die Postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren:

- **Einzelbenutzer**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Organisation**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Weitere Informationen finden [Sie unter Verwalten der Postfachüberwachung](https://go.microsoft.com/fwlink/?linkid=2103668).