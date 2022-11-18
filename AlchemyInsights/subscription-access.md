---
title: Abonnementzugriff
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 9a93bedb2a32dbc87b239fc9261b775631160516
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66425254"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Azure kann aufgrund von Browserproblemen nicht angemeldet werden (Browser hängt, dreht sich weiter, wird nicht geladen usw.)

Möglicherweise sind Sie von einem Ausfall betroffen. Überprüfen Sie, ob es einen laufenden Ausfall gibt: [Azure-Integritätsstatus](https://status.azure.com/status/history/).

Melden Sie sich bei allen aktiven Azure-Sitzungen ab. Starten Sie einen inprivaten oder inkognito-Modus Ihres Webbrowsers.

Sie können auch versuchen, den Browser zu aktualisieren, einen anderen Browser zu verwenden und Cachecookies zu löschen, wenn oben nicht funktioniert.

Weitere Informationen: [Behandeln von Anmeldeproblemen](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Auf Abonnements kann nicht zugegriffen werden.**

Stellen Sie in der [Azure-Portal](https://portal.azure.com/) sicher, dass das richtige Azure-Verzeichnis aus dem Konto oben rechts ausgewählt ist.

Stellen Sie im [Azure Account Center](https://account.windowsazure.com/Subscriptions) sicher, dass es sich bei dem verwendeten Konto um den Kontoadministrator handelt.

Weitere Informationen: [Problembehandlung bei "Keine Abonnements gefunden](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)"

**Auf den Abrechnungsverlauf kann nicht zugegriffen werden.**

Der Kontoadministrator muss sicherstellen, dass der Benutzer, der auf die Abrechnungsinformationen zugreift, im Azure Active Directory als Gastbenutzer hinzugefügt wird: [Hinzufügen oder Löschen eines neuen Benutzers](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Dem Benutzer muss dann eine globale Administratorrolle zugewiesen werden: [Benutzerrolle zuweisen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Danach kann dem Benutzer mithilfe von RBAC-Richtlinien Abrechnungszugriff gewährt werden: [Gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Empfohlene Dokumentationen**

-   [Ich kann mich nicht anmelden, um mein Azure-Abonnement zu verwalten.](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)