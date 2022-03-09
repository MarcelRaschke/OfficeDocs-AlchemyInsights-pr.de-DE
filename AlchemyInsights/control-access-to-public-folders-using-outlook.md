---
title: Steuern des Zugriffs auf Öffentliche Ordner mit Outlook
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: bde031c1d562d402e2ac3721d3b8637ed9970489
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63240137"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Steuern des Zugriffs auf Öffentliche Ordner mit Outlook

So steuern Sie, welche Benutzer über Outlook auf Öffentliche Ordner zugreifen können:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` verwenden

$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Hinweis: Mit diesem Verfahren können nur Verbindungen mit dem Outlook-Desktop für Windows-Clients gesteuert werden. Benutzer können weiterhin mit OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.

Weitere Informationen hierzu finden Sie unter [Kontrollierte Verbindungen zu Öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).
