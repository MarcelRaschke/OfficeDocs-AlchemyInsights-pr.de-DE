---
title: ClientAccessServerEnabled auf True festlegen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000078"
- "7342"
ms.date: 02/24/2021
ms.openlocfilehash: 8fb43c96f72fcd8c0db87523ae970d34fddb6d98
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66325659"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled auf True festlegen

Wenn Sie eine verschlüsselte E-Mail-Nachricht nicht öffnen können und **stattdessen eine rpmsg-Anlage** sehen können, führen Sie die folgenden Schritte aus:

1. Stellen Sie eine Verbindung mit Exchange Online PowerShell her.

    **Hinweis**: Um eine Verbindung mit Exchange Online PowerShell herzustellen, müssen Sie sich mit einem globalen Administrator- oder Exchange-Administratorkonto anmelden.

   a. Öffnen Sie Windows PowerShell, und führen Sie dann den folgenden Befehl aus:`$UserCredential = Get-Credential`
   b. Geben Sie im Dialogfeld **Windows PowerShell Anmeldeinformationsanforderung** Ihr Geschäfts-, Schul- oder Unikonto und Das Kennwort c ein. Klicken Sie auf **OK**. 

2. Führen Sie den folgenden Befehl aus, um eine neue Sitzung zu erstellen:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Führen Sie den folgenden Befehl aus:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Befehl ausführen `Get-IRMConfiguration` .

4. Überprüfen Sie die Einstellung **"ClientAccessServerEnabled** ". 

    a. Wenn **die Einstellung "ClientAccessServerEnabled** " auf **"False**" festgelegt ist, führen Sie das folgende Cmdlet aus: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tipp**: Schließen Sie Ihre PowerShell-Sitzung immer mit dem folgenden Befehl: `Remove-PSSession $Session`

Weitere Informationen finden Sie [unter Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

