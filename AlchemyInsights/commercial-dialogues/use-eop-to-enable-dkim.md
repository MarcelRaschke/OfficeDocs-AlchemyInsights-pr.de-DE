---
title: Verwenden Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9002531"
- "7375"
ms.date: 02/23/2021
ms.openlocfilehash: 9f4caf967e24f9042a68f950ee32f1aa94236bfe
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66368211"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Verwenden Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne

Wenn Sie die DKIM-DNS-Einträge im Admin Center nicht erstellen können, verwenden Sie Exchange Online PowerShell. 

Führen Sie die folgenden Schritte aus, um einen DKIM-DNS-Eintrag mit Exchange Online PowerShell zu erstellen:

1. Öffnen Sie Windows PowerShell als Administrator, und führen Sie die folgenden Befehle in der beschriebenen Reihenfolge aus:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Wenn Sie Probleme beim Herstellen einer Verbindung mit Exchange Online PowerShell haben, lesen Sie ["Verbinden mit Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)".

2. Nachdem Sie mit Exchange Online PowerShell verbunden sind, führen Sie den folgenden Befehl aus:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Nachdem der obige Befehl erfolgreich ausgeführt wurde, führen Sie den folgenden Befehl aus, um die Exchange Online PowerShell-Sitzung zu beenden:

    `Remove-PSSession $Session` 



