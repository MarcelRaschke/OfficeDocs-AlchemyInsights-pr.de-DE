---
title: Kein Zugriff auf öffentliche Ordner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996629"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook keine Verbindung mit öffentlichen Ordnern herstellen

Wenn der Zugriff auf öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Verbinden zu EXO PowerShell, und konfigurieren Sie den DefaultPublicFolderMailbox-Parameter für das problematische Benutzerkonto so, dass er mit dem Parameter für ein funktionierendes Benutzerkonto übereinstimmt.

Beispiel:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin besteht, führen Sie [dieses Verfahren](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf öffentliche Ordner mithilfe von Outlook zu beheben.
 
**So steuern Sie, welche Benutzer über Outlook auf öffentliche Ordner zugreifen können:**

1.  Verwenden Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true oder $false  
      
    $true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
      
    $false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Hinweis** Dieses Verfahren kann Verbindungen nur mit Outlook Desktop für Windows Clients steuern. Ein Benutzer kann weiterhin mithilfe von OWA oder Outlook für Mac auf öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie unter Ankündigung der [Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).