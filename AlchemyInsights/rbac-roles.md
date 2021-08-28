---
title: 'RBAC-Rollen '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923130"
---
# <a name="rbac-rules"></a>RBAC-Regeln

Wenn Sie den Berechtigungsfehler erhalten: 

- **Der Client mit Objekt-ID verfügt nicht über die Autorisierung zum Ausführen von Aktionen über den Bereich (Code: AuthorizationFailed):** Wenn Sie versuchen, eine Ressource zu erstellen, überprüfen Sie, ob Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über Schreibberechtigungen für die Ressource im ausgewählten Bereich verfügt. Um beispielsweise virtuelle Computer in einer Ressourcengruppe zu verwalten, sollten Sie über die Rolle ["Mitwirkender](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) für virtuelle Computer" in der Ressourcengruppe (oder dem übergeordneten Bereich) verfügen. Eine Liste der Berechtigungen für jede integrierte Rolle finden Sie unter ["Integrierte Rollen für Azure-Ressourcen".](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Sie verfügen nicht über die Berechtigung zum Erstellen einer Supportanfrage:** Wenn Sie versuchen, ein Supportticket zu erstellen oder zu aktualisieren, überprüfen Sie, ob Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle mit der Berechtigung "Microsoft.Support/supportTickets/write" zugewiesen ist, z. B. [Mitwirkender für Supportanfragen.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- **Es können keine Rollenzuweisungen mehr erstellt werden (Code: RoleAssignmentLimitExceeded):** Wenn Sie versuchen, eine Rolle zuzuweisen, versuchen Sie, die Anzahl der Rollenzuweisungen zu reduzieren, indem Sie stattdessen Gruppen Rollen zuweisen. Azure unterstützt bis zu **2.000** Rollenzuweisungen pro Abonnement.

Weitere Informationen zu Azure RBAC-Rollen finden Sie unter [Azure RBAC-Rollen.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
