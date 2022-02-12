---
title: 451 4.7.0 Temporärer Serverfehler. Wiederholen Sie den Vorgang zu einem späteren Zeitpunkt. PRX4
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: 7cf9a73f581f494845c68a57a811b60a5e863f3c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62567415"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Temporärer Serverfehler. Wiederholen Sie den Vorgang zu einem späteren Zeitpunkt. PRX4

Beim Senden von E-Mails über Smarthost "smtp.office365.com" mithilfe der SMTP-Clientübermittlungsmethode tritt möglicherweise ein Problem auf und sie erhalten den Fehler: "451 4.7.0 Temporärer Serverfehler. Wiederholen Sie den Vorgang zu einem späteren Zeitpunkt. PRX4 ist meist temporär." 

Stellen Sie sicher, dass Sie kein freigegebenes Postfach für die SMTP-Clientübermittlung verwenden, da für die SMTP-Clientübermittlungsmethode ein lizenziertes Postfach zum Senden von E-Mails erforderlich ist. Wenn Sie jedoch kein freigegebenes Postfach verwenden und das Problem weiterhin besteht, überprüfen Sie Folgendes:

1. Aktivieren Sie die Client-SMTP-Übermittlung für das lizenzierte Postfach, das mithilfe dieses PowerShell-Befehls verwendet wird:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OR

    1. Wechseln Sie zu Microsoft 365 Admin Center > **Aktive Benutzer**, und wählen Sie den Benutzer aus.
    1. Wechseln Sie zur Registerkarte " **E-Mail" > E-Mail-Apps** > wählen **Sie "E-Mail-Apps verwalten" aus**. 
    1. Stellen Sie sicher, dass die **Einstellung für authentifizierte SMTP** aktiviert ist.
    1. Wählen Sie **Änderungen speichern** aus.
    
    Führen Sie den folgenden Befehl aus, um die SMTP-Authentifizierung für eine gesamte Organisation zu aktivieren:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Hinweis**: Aus Sicherheitsgründen wird empfohlen, die SMTP-Authentifizierung nur für das verwendete Postfach zu aktivieren. Die Einstellung auf Benutzerebene setzt die Einstellung auf Organisationsebene außer Kraft.

2. Deaktivieren Sie die Azure-Sicherheitsstandards, indem **Sie die Standardsicherheitseinstellungen** aktivieren auf **"Nein**" umschalten:

    1. Melden Sie sich beim Azure-Portal als Sicherheitsadministrator, Administrator für bedingten Zugriff oder globaler Administrator an.
    1. Navigieren Sie zu Azure Active Directory >** Eigenschaften**, und wählen Sie **"Sicherheitsstandards verwalten" aus**.
    1. Legen Sie die Option " **Standardsicherheit aktivieren** " auf **"Nein**" fest.
    1. Wählen Sie **Speichern**.

3. Deaktivieren Sie die mehrstufige Authentifizierung (Multi Factor Authentication, MFA) für das lizenzierte Postfach, das verwendet wird.

    1. Wechseln Sie zum Microsoft 365 Admin Center, und wählen Sie im linken Navigationsmenü **"UsersActive** > **"-Benutzer** aus.
    1. Wählen Sie auf der Seite **Aktive Benutzer** die Option **Mehrstufige Authentifizierung** aus.
    1. Wählen Sie den Benutzer aus, und deaktivieren Sie **die mehrstufige Authentifizierung**.

