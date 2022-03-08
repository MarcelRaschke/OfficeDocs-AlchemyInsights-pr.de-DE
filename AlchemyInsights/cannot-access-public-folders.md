---
title: Kein Zugriff auf öffentliche Ordner
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 8ed08b706ecc25a9022b7771f43fefc1d2936802
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63208148"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook keine Verbindung mit öffentlichen Ordnern herstellen

Wenn der Zugriff auf öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Verbinden zu EXO PowerShell, und konfigurieren Sie den DefaultPublicFolderMailbox-Parameter für das problematische Benutzerkonto so, dass er dem Parameter für ein funktionierendes Benutzerkonto entspricht.

Beispiel:

`Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox`

`Set-Mailbox ProblemUser -DefaultPublicFolderMailbox <value from previous command>`

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin besteht, führen Sie [dieses Verfahren](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf öffentliche Ordner mithilfe von Outlook zu beheben.

**So steuern Sie, welche Benutzer über Outlook auf öffentliche Ordner zugreifen können**:

1. Verwenden oder `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true``$false`  

    `$true`: Benutzern den Zugriff auf öffentliche Ordner in Outlook

    `$false`: Benutzerzugriff auf öffentliche Ordner in Outlook verhindern. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

**Hinweis** Dieses Verfahren kann Verbindungen nur mit Outlook Desktop für Windows Clients steuern. Ein Benutzer kann weiterhin mithilfe von OWA oder Outlook für Mac auf öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie unter [Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).