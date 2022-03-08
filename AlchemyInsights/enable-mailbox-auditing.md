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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 31a806e1e199d4140897593fee494995d09315c1
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63092134"
---
# <a name="enable-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Um die Postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, müssen die folgenden Cmdlets über die Remote-PowerShell ausgeführt werden:
  
 **Einzelner Benutzer**
  
Set-Mailbox -Identity "Jane Maustaste" -AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Weitere Informationen](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

