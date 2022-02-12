---
title: Steuern des Zugriffs auf Öffentliche Ordner mit Outlook
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 3fef8ea10c335c33c8398c346bbaeb18a6d1e45b
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62654466"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Steuern des Zugriffs auf Öffentliche Ordner mit Outlook

So steuern Sie, welche Benutzer über Outlook auf Öffentliche Ordner zugreifen können:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` verwenden

$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Hinweis: Mit diesem Verfahren können nur Verbindungen mit dem Outlook-Desktop für Windows-Clients gesteuert werden. Benutzer können weiterhin mit OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.

Weitere Informationen hierzu finden Sie unter [Kontrollierte Verbindungen zu Öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).
