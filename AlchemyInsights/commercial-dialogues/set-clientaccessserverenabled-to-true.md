---
title: Festlegen von "ClientAccessServerEnabled" auf "True"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: c620eb4c8ef78de8c7fcd780947e87b4c3c05d55
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62641344"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Festlegen von "ClientAccessServerEnabled" auf "True"

Wenn Sie eine verschlüsselte E-Mail-Nachricht nicht öffnen können und stattdessen eine **Rpmsg-Anlage** sehen, führen Sie die folgenden Schritte aus:

1. Stellen Sie eine Verbindung mit Exchange Online PowerShell her.

    **Hinweis**: Um eine Verbindung mit Exchange Online PowerShell herzustellen, müssen Sie sich mit einem globalen Administratorkonto oder Exchange Administratorkonto anmelden.

   a. Öffnen Sie Windows PowerShell, und führen Sie dann den folgenden Befehl aus:`$UserCredential = Get-Credential`
   b. Geben Sie im Dialogfeld **Windows PowerShell Anmeldeinformationsanforderung** Ihr Geschäfts-, Schul- oder Unikonto und Kennwort ein, c. Klicken Sie auf **OK**. 

2. Führen Sie den folgenden Befehl aus, um eine neue Sitzung zu erstellen:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Führen Sie den folgenden Befehl aus:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Führen Sie den Befehl aus `Get-IRMConfiguration` .

4. Überprüfen Sie die **Einstellung "ClientAccessServerEnabled** ". 

    a. Wenn die Einstellung **"ClientAccessServerEnabled** " auf **"False"** festgelegt ist, führen Sie das folgende Cmdlet aus: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tipp**: Schließen Sie Ihre PowerShell-Sitzung immer mit dem folgenden Befehl: `Remove-PSSession $Session`

Weitere Informationen finden Sie unter [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

