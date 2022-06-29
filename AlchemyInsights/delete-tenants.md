---
title: Mandanten löschen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003256"
- "7297"
ms.date: 11/23/2020
ms.openlocfilehash: 62a046e46182a5917295ae0bf5efdc02a90d2109
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66324255"
---
# <a name="delete-tenant"></a>Mandanten löschen

Stellen Sie zum Löschen eines Azure AD Folgendes sicher:
- Sie sind ein globaler Administrator im Verzeichnis.
- Sie sind NICHT mit einem Konto angemeldet, das über das Standardverzeichnis verfügt, z. B. contoso.onmicrosoft.com im angemeldeten Konto, z. B. admin@contoso.onmicrosoft.com.
- Entfernen Sie alle aktiven Anwendungen im Verzeichnis vor dem Löschen. Um aktive Anwendungen zu entfernen, navigieren Sie zu App-Registrierungen und entfernen Sie die vorhandenen Anwendungen.
- Es sind keine aktiven Abonnements für Microsoft Online-Dienste wie Microsoft Azure, Office 365 oder Azure AD Premium im Verzeichnis zugeordnet. Übertragen Sie Ihre Abonnements oder beschleunigen Sie die Kündigung aktiver Abonnements über Azure Support und Abrechnung. Weitere Informationen zum Kündigen von Office 365- und Azure-Abonnements. Anleitungen zum Zuordnen oder Hinzufügen eines vorhandenen Abonnements zu einem Mandanten finden Sie unter [Zuordnen oder Hinzufügen eines Azure-Abonnements zu Ihrem Azure AD-Mandanten](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Es gibt keine aktive Lizenz. Informationen zum Entfernen von Lizenzen finden Sie unter [Entfernen des Abonnements zum Entfernen der Lizenz](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Es gibt keine anderen aktiven Benutzer im Verzeichnis neben Sich selbst als globaler Administrator, wenn Sie versuchen, Azure AD zu löschen. Entfernen Sie alle anderen aktiven Benutzer, und alle Abhängigkeiten von einem benutzerdefinierten Domänennamen im Mandanten müssen ebenfalls entfernt werden, z. B. Benutzer, die mit admin@contoso.com erstellt wurden.

Ausführlichere Schritte zur Vorgehensweise:
- Löschen Sie "Azure Active Directory" oder "Abonnement", siehe ["Löschen von Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)".
- Entfernen von Anwendungen im Verzeichnis finden [Sie unter Entfernen von Anwendungen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
