---
title: Einrichten oder Entfernen der E-Mail-Weiterleitung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1200004"
- "20"
ms.date: 07/28/2022
ms.openlocfilehash: 8383e25abfe1c6050a9e92c0947db20c00742e40
ms.sourcegitcommit: b7ec572b250ab6a4e140e36a64db063df3e55c24
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2022
ms.locfileid: "67070552"
---
# <a name="set-up-or-remove-email-forwarding"></a>Einrichten oder Entfernen der E-Mail-Weiterleitung

Auf Mandantenebene können Sie die externe Weiterleitung mithilfe der ausgehenden Spamrichtlinie steuern. Überprüfen Sie die Ausgehende Spamfilterrichtlinie von Microsoft 365 Defender > **Email & Richtlinien für die Zusammenarbeit** > **und Regeln** > **für Bedrohungsrichtlinien** > [**Antispam**](https://security.microsoft.com/antispam) oder mithilfe des Befehls [`Get-HostedOutboundSpamFilterPolicy`](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy). Wenn der Block auf Mandantenebene eingerichtet ist, erhalten Benutzer die Fehlermeldung "550 5.7.520 Zugriff verweigert, Ihre Organisation lässt keine externe Weiterleitung zu."

Wenn Sie zulassen möchten, dass einige Benutzer die automatische externe E-Mail-Weiterleitung fortsetzen können, erstellen Sie eine neue ausgehende Spamrichtlinie, oder ändern Sie die vorhandene Richtlinie so, dass sie die zuzulassenden Benutzer oder Domänen enthält. Die Option zum Zulassen von Gruppen ist nicht verfügbar. Ausführliche Informationen finden Sie [unter Steuern der automatischen externen E-Mail-Weiterleitung in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).

**Hinweis**: Es wird empfohlen, die automatische externe E-Mail-Weiterleitung in Ihrer standardmäßigen ausgehenden Spamfilterrichtlinie zu deaktivieren und nur für die Benutzer zu aktivieren, die externe Weiterleitung benötigen, indem Sie eine benutzerdefinierte Richtlinie für diese Benutzer erstellen. 

So überprüfen Sie die E-Mail-Weiterleitungseinstellungen für ein Postfach:

- Wenn es sich um ein Benutzerpostfach handelt, wechseln Sie zu "**Aktive Benutzer****"** > , und wählen Sie den Benutzer aus, dessen Postfach Sie weiterleiten möchten. Wählen Sie auf der Registerkarte **E-Mail** die Option **E-Mail-Weiterleitung verwalten** aus.

- Wenn es sich um ein freigegebenes Postfach handelt, wechseln Sie zu **"Freigegebene Gruppenpostfächer** > ", und wählen Sie das freigegebene Postfach aus, das Sie weiterleiten möchten. Wählen Sie **Bearbeiten** aus.

Weitere Informationen finden Sie unter [Konfigurieren der E-Mail-Weiterleitung in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding). .

Anweisungen, die Benutzer zum Einrichten der E-Mail-Weiterleitung in ihren eigenen Postfächern verwenden können, finden Sie unter ["Weiterleiten von E-Mails von Microsoft 365 an ein anderes E-Mail-Konto](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)". Beachten Sie, dass Sie E-Mails nur an eine E-Mail-Adresse weiterleiten können. Wenn Sie die Weiterleitung an eine Gruppe von Personen einrichten müssen, erstellen Sie eine Verteilerliste (unter **"Gruppen**"), fügen Sie Ihre Benutzer hinzu, und konfigurieren Sie dann die Weiterleitung an die neue Gruppe.

Verlässt ein Mitarbeiter die Organisation? Empfohlene Schritte zum Entfernen aus Microsoft 365 finden Sie unter [Übersicht: Entfernen eines ehemaligen Mitarbeiters und sicherer Daten](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee).