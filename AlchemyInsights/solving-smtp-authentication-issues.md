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
ms.openlocfilehash: b81ae4a96708858d868d1fea1905c5858083c2fa
ms.sourcegitcommit: 5afc3c4a1270409ed3691c90ba139878d845e7a3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/10/2022
ms.locfileid: "66007373"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Aktivieren von SMTP-Authentifizierung und Problembehandlung

Wenn Sie die SMTP-Authentifizierung für ein Postfach aktivieren möchten oder beim Versuch, E-Mails durch Authentifizierung eines Geräts oder einer Anwendung bei Microsoft 365 weiterzuleiten, eine Fehlermeldung wie „Client nicht authentifiziert“, „Authentifizierung nicht erfolgreich“ oder „SmtpClientAuthentication“ mit Code 5.7.57, 5.7.3 oder 5.7.139 erhalten, führen Sie die folgenden drei Aktionen durch, um das Problem zu beheben:

1. Deaktivieren Sie die [Azure-Sicherheitsstandards](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), indem Sie die Option **Sicherheitsstandards aktivieren** auf **Nein** festlegen.

    1. Melden Sie sich beim Azure-Portal als Sicherheitsadministrator, Administrator für bedingten Zugriff oder globaler Administrator an.
    2. Navigieren Sie zu Azure Active Directory > **Eigenschaften**.
    3. Wählen Sie **Sicherheitsstandards verwalten** aus.
    4. Legen Sie **Sicherheitsstandards aktivieren** auf **Nein** fest.
    5. Wählen Sie **Speichern** aus.

2. [Aktivieren Sie die SMTP-Clientübermittlung](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) für das lizenzierte Postfach.

    1. Navigieren Sie im Microsoft 365 Admin Center zu [**Aktive Benutzer**](https://admin.microsoft.com/AdminPortal/Home?ref=users), und wählen Sie den Benutzer aus.
    2. Navigieren Sie zur Registerkarte „E-Mail“, und wählen Sie unter **E-Mail-Apps** die Option **E-Mail-Apps verwalten** aus.
    3. Stellen Sie sicher, dass **Authentifiziertes SMTP** ausgewählt (aktiviert) ist.
    4. Wählen Sie **Änderungen speichern** aus.

3. [Deaktivieren Sie die mehrstufige Authentifizierung (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) für das lizenzierte Postfach.

    1. Gehen Sie zum Microsoft 365 Admin Center, und wählen Sie im linken Navigationsmenü **Benutzer** > [**Aktive Benutzer**](https://admin.microsoft.com/AdminPortal/Home?ref=users) aus.
    2. Wählen Sie **Mehrstufige Authentifizierung** aus.
    3. Wählen Sie den Benutzer aus, und deaktivieren Sie **Mehrstufige Authentifizierung**.
