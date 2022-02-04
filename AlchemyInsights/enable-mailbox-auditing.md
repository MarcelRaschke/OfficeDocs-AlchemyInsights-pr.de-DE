---
title: Aktivieren der Postfachüberwachung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 8727d3e19a671e04eb2582f5c2cbb379b3bd5e8a
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61934352"
---
# <a name="enable-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Um die Postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, müssen die folgenden Cmdlets über die Remote-PowerShell ausgeführt werden:
  
 **Einzelner Benutzer**
  
Set-Mailbox -Identity "Jane Maustaste" -AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Weitere Informationen](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

