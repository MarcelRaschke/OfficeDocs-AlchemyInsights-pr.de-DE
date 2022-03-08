---
title: Verwenden Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 9b37c6793cd8346d098e2811e4816ebf80f59128
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63216789"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Verwenden Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne

Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, versuchen Sie, Exchange Online PowerShell zu verwenden. 

Führen Sie die folgenden Schritte aus, um einen DKIM-DNS-Eintrag mit Exchange Online PowerShell zu erstellen:

1. Öffnen Sie Windows PowerShell als Administrator, und führen Sie die folgenden Befehle in der beschriebenen Sequenz aus:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Wenn Sie Probleme beim Herstellen einer Verbindung mit Exchange Online PowerShell haben, lesen Sie [Verbinden zu Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Nachdem Sie mit Exchange Online PowerShell verbunden sind, führen Sie den folgenden Befehl aus:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Nachdem der oben genannte Befehl erfolgreich ausgeführt wurde, führen Sie den folgenden Befehl aus, um die Exchange Online PowerShell-Sitzung zu beenden:

    `Remove-PSSession $Session` 



