---
title: Mandant löschen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: b621622a1234764c35c526c7b0cc9adb557015e4
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63185900"
---
# <a name="delete-tenant"></a>Mandant löschen

Um eine Azure AD zu löschen, stellen Sie Folgendes sicher:
- Sie sind ein globaler Administrator im Verzeichnis.
- Sie sind NICHT mit einem Konto angemeldet, das über das Standardverzeichnis verfügt, z. B. contoso.onmicrosoft.com im angemeldeten Konto, z. B. admin@contoso.onmicrosoft.com.
- Entfernen Sie alle aktiven Anwendungen im Verzeichnis vor dem Löschen. Um aktive Anwendungen zu entfernen, navigieren Sie zu App-Registrierungen, und entfernen Sie die vorhandenen Anwendungen.
- Es gibt keine aktiven Abonnements für Microsoft Online Services, z. B. Microsoft Azure, Office 365 oder Azure AD Premium, die dem Verzeichnis zugeordnet sind. Übertragen Sie Ihre Abonnements oder beschleunigen Sie die Kündigung aktiver Abonnements über Azure-Support und Abrechnung. Erfahren Sie mehr über das Kündigen von Office 365 und Azure-Abonnements. Anleitungen zum Zuordnen oder Hinzufügen eines vorhandenen Abonnements zu einem Mandanten finden Sie unter [Zuordnen oder Hinzufügen eines Azure-Abonnements zu Ihrem Azure AD Mandanten](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Es gibt keine aktive Lizenz. Informationen zum Entfernen von Lizenzen finden Sie unter ["Entfernen von Abonnements zum Entfernen von Lizenzen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)".
- Es befinden sich keine anderen aktiven Benutzer im Verzeichnis als der globale Administrator, wenn Sie versuchen, die Azure AD zu löschen. Entfernen Sie alle anderen aktiven Benutzer, und alle Abhängigkeiten von einem benutzerdefinierten Domänennamen im Mandanten müssen ebenfalls entfernt werden, z. B. Benutzer, die mit admin@contoso.com erstellt wurden.

Weitere Details finden Sie in den folgenden Schritten:
- Löschen Sie "Azure Active Directory" oder "Abonnement", siehe ["Löschen Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)".
- Entfernen von Anwendungen im Verzeichnis, siehe ["Entfernen von Anwendungen"](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
