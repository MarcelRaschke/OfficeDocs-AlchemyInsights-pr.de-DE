---
title: Abonnementzugriff
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999239"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Anmelden in Azure aufgrund von Browserproblemen nicht möglich (Browser hängt an, dreht sich weiter, lädt nicht usw.)

Möglicherweise sind Sie von einem Ausfall betroffen. Überprüfen Sie, ob ein fortlaufender Ausfall vorliegt: [Azure Health Status](https://status.azure.com/status/history/).

Melden Sie sich bei allen aktiven Azure-Sitzungen ab. Starten Sie einen privaten oder inkognito-Modus Ihres Webbrowsers.

Sie können auch versuchen, den Browser zu aktualisieren, einen anderen Browser zu verwenden und Cachecookies zu löschen, wenn dies oben nicht funktioniert.

Weitere Informationen: [Behandeln von Anmeldeproblemen](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Zugriff auf Abonnements nicht möglich**

Stellen Sie im [Azure-Portal](https://portal.azure.com/)sicher, dass das richtige Azure-Verzeichnis aus dem Konto oben rechts ausgewählt ist.

Stellen Sie im [Azure-Kontocenter](https://account.windowsazure.com/Subscriptions)sicher, dass das verwendete Konto der Kontoadministrator ist.

Weitere Informationen: [Problembehandlung ohne gefundene Abonnements](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zugriff auf Abrechnungsverlauf nicht möglich**

Der Kontoadministrator muss sicherstellen, dass der Benutzer, der auf die Abrechnungsinformationen zugreift, im Azure Active Directory als Gastbenutzer hinzugefügt wird: [Hinzufügen oder Löschen eines neuen Benutzers.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Dem Benutzer muss dann eine globale Administratorrolle zugewiesen werden: [Benutzern eine Rolle zuweisen.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

In diesem Fall kann dem Benutzer der Zugriff auf die Abrechnung mithilfe von RBAC-Richtlinien gewährt werden: Gewähren des [Zugriffs auf die Abrechnung.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Empfohlene Dokumente**

-   [Ich kann mich nicht anmelden, um mein Azure-Abonnement zu verwalten.](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)