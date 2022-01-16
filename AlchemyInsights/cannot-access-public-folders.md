---
title: Kein Zugriff auf öffentliche Ordner
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: b63a3912a9f8ee41e7c7b73e0ce97b29a42fe3e6
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61956300"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook keine Verbindung mit öffentlichen Ordnern herstellen

Wenn der Zugriff auf öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Verbinden zu EXO PowerShell, und konfigurieren Sie den DefaultPublicFolderMailbox-Parameter für das problematische Benutzerkonto so, dass er dem Parameter für ein funktionierendes Benutzerkonto entspricht.

Beispiel:

`Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox`

`Set-Mailbox ProblemUser -DefaultPublicFolderMailbox <value from previous command>`

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin besteht, führen Sie [dieses Verfahren](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf öffentliche Ordner mithilfe von Outlook zu beheben.

**So steuern Sie, welche Benutzer über Outlook auf öffentliche Ordner zugreifen können:**

1. Verwenden `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true` oder `$false`  

    `$true`: Benutzern den Zugriff auf öffentliche Ordner in Outlook

    `$false`: Benutzerzugriff auf öffentliche Ordner in Outlook verhindern. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

**Hinweis** Dieses Verfahren kann Verbindungen nur mit Outlook Desktop für Windows Clients steuern. Ein Benutzer kann weiterhin mit OWA oder Outlook für Mac auf öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie unter Ankündigung der [Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).