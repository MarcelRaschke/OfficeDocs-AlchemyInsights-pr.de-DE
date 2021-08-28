---
title: Die Standardauthentifizierung für Exchange PowerShell wird eingestellt
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069243"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Die Standardauthentifizierung für Exchange PowerShell wird eingestellt

Die neuesten Informationen darüber, wie eine Verbindung zu Exchange Online PowerShell ohne Verwendung der Standardauthentifizierung hergestellt werden kann, [finden Sie hier](https://aka.ms/exops-docs). Im PowerShell V2-Modul wird keine Standardauthentifizierung verwendet.

Beachten Sie, dass auf dem Clientcomputer weiterhin die Standardauthentifizierung aktiviert sein muss.
Das neue PowerShell V2-Modul verwendet moderne Authentifizierung, um eine Verbindung zum Aktivieren aller REST-basierten V2-Cmdlets herzustellen. Zusätzlich zu den V2-Cmdlets ermöglicht es Ihnen auch den Zugriff auf ältere Remote-PowerShell-Cmdlets (RPS), für die eine PowerShell-Remotesitzung eingerichtet werden muss. Zum Einrichten einer RPS-Sitzung auf einem Windows-Computer muss WinRM BasicAuth auf dem Clientcomputer aktiviert werden, auch wenn das Modul einen modernen Authentifizierungsmechanismus für den Dienst verwendet. Die WinRM-Standardauthentifizierungspipeline wird für den Transport moderner Authentifizierungstoken verwendet. Wenn die WinRM-Standardauthentifizierung auf dem Clientcomputer deaktiviert ist, funktionieren die neuen V2-Cmdlets weiterhin (aber die alten RPS-Cmdlets nicht).
