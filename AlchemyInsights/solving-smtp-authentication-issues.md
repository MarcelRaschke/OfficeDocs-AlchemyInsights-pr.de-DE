---
title: Aktivieren von SMTP-Authentifizierung und Problembehandlung
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
- "3000003"
- "5652"
ms.openlocfilehash: 27b32b361824a0d670544f53964a3fcc1026eb14
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63291411"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Aktivieren von SMTP-Authentifizierung und Problembehandlung

Wenn Sie die SMTP-Authentifizierung für ein Postfach aktivieren möchten oder beim Versuch, E-Mails durch Authentifizierung eines Geräts oder einer Anwendung bei Microsoft 365 weiterzuleiten, eine Fehlermeldung wie „Client nicht authentifiziert“, „Authentifizierung nicht erfolgreich“ oder „SmtpClientAuthentication“ mit Code 5.7.57, 5.7.3 oder 5.7.139 erhalten, führen Sie die folgenden drei Aktionen durch, um das Problem zu beheben:

1. Deaktivieren Sie die [Azure-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), indem Sie die Option **Sicherheitsstandards aktivieren** auf **Nein** festlegen.

    a. Melden Sie sich beim Azure-Portal als Sicherheitsadministrator, Administrator für bedingten Zugriff oder globaler Administrator an.<BR/>
    a. Navigieren Sie zu Azure Active Directory > **Eigenschaften**.<BR/>
    c. Wählen Sie **Sicherheitsstandards verwalten** aus.<BR/>
    d. Legen Sie **Sicherheitsstandardwerte aktivieren** auf **Nein** fest.<BR/>
    e. Wählen Sie **Speichern** aus.

2. [Aktivieren Sie die SMTP-Clientübermittlung](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) für das lizenzierte Postfach.

    a. Wechseln Sie im Microsoft 365 Admin Center zu **Aktive Benutzer**, und wählen Sie den Benutzer aus.<BR/>
    b. Wechseln Sie zur Registerkarte "E-Mail", und wählen Sie unter **E-Mail-Apps****E-Mail-Apps verwalten** aus.<BR/>
    d. Stellen Sie sicher, dass **Authentifiziertes SMTP** aktiviert ist.<BR/>
    e. Wählen Sie **Änderungen speichern** aus.<BR/>

3. [Deaktivieren Sie die mehrstufige Authentifizierung (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) für das lizenzierte Postfach.

    a. Wechseln Sie zum Microsoft 365 Admin Center, und wählen Sie im linken Navigationsmenü **Benutzer** > **Aktive Benutzer** aus.<BR/>
    b. Wählen Sie **Mehrstufige Authentifizierung** aus.<BR/>
    c. Wählen Sie den Benutzer aus, und deaktivieren Sie **Mehrstufige Authentifizierung**.<BR/>
