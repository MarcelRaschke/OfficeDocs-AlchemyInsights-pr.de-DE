---
title: Die Standardauthentifizierung für Exchange PowerShell wird eingestellt
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
- "3500011"
- "4577"
ms.openlocfilehash: f99970b02c251b15a0d47e2debf7c1a34294caa9
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61969051"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Die Standardauthentifizierung für Exchange PowerShell wird eingestellt

Die neuesten Informationen darüber, wie eine Verbindung zu Exchange Online PowerShell ohne Verwendung der Standardauthentifizierung hergestellt werden kann, [finden Sie hier](https://aka.ms/exops-docs). Im PowerShell V2-Modul wird keine Standardauthentifizierung verwendet.

Beachten Sie, dass auf dem Clientcomputer weiterhin die Standardauthentifizierung aktiviert sein muss.
Das neue PowerShell V2-Modul verwendet moderne Authentifizierung, um eine Verbindung zum Aktivieren aller REST-basierten V2-Cmdlets herzustellen. Zusätzlich zu den V2-Cmdlets ermöglicht es Ihnen auch den Zugriff auf ältere Remote-PowerShell-Cmdlets (RPS), für die eine PowerShell-Remotesitzung eingerichtet werden muss. Zum Einrichten einer RPS-Sitzung auf einem Windows-Computer muss WinRM BasicAuth auf dem Clientcomputer aktiviert werden, auch wenn das Modul einen modernen Authentifizierungsmechanismus für den Dienst verwendet. Die WinRM-Standardauthentifizierungspipeline wird für den Transport moderner Authentifizierungstoken verwendet. Wenn die WinRM-Standardauthentifizierung auf dem Clientcomputer deaktiviert ist, funktionieren die neuen V2-Cmdlets weiterhin (aber die alten RPS-Cmdlets nicht).
