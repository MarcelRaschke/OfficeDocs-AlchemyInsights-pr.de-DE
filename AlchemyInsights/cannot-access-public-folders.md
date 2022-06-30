---
title: Auf öffentliche Ordner kann nicht zugegriffen werden.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 2911e8213271e7061cec08cdcfe43246faeb7939
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66381261"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kann keine Verbindung mit öffentlichen Ordnern herstellen.

Wenn der Zugriff auf öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Stellen Sie eine Verbindung mit EXO PowerShell her, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das problembehebungsbenutzerkonto so, dass er mit dem Parameter für ein funktionierendes Benutzerkonto übereinstimmt.

Beispiel:

`Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox`

`Set-Mailbox ProblemUser -DefaultPublicFolderMailbox <value from previous command>`

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin besteht, führen Sie [dieses Verfahren](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf öffentliche Ordner mitHilfe von Outlook zu beheben.

**So steuern Sie, welche Benutzer mitHilfe von Outlook auf öffentliche Ordner zugreifen können**:

1. Verwenden `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true` oder `$false`  

    `$true`: Zulassen, dass Benutzer auf öffentliche Ordner in Outlook zugreifen können

    `$false`: Verhindern des Benutzerzugriffs auf öffentliche Ordner in Outlook. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

**Hinweis** Dieses Verfahren kann Verbindungen nur mit Outlook-Desktop für Windows-Clients steuern. Ein Benutzer kann weiterhin mithilfe von OWA oder Outlook für Mac auf öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie [unter Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).