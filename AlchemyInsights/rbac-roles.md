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
ms.openlocfilehash: 22bf26fd8fb81cf25976a4ff47568a0b8dfc78f6
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62680063"
---
# <a name="rbac-rules"></a>RBAC-Regeln

Wenn Sie den Berechtigungsfehler erhalten: 

- **Der Client mit Objekt-ID verfügt nicht über die Autorisierung zum Ausführen von Aktionen über den Bereich (Code: AuthorizationFailed):** Wenn Sie versuchen, eine Ressource zu erstellen, überprüfen Sie, ob Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über Schreibberechtigungen für die Ressource im ausgewählten Bereich verfügt. Um beispielsweise virtuelle Computer in einer Ressourcengruppe zu verwalten, sollten Sie über die Rolle " [Mitwirkender für virtuelle Computer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) " in der Ressourcengruppe (oder dem übergeordneten Bereich) verfügen. Eine Liste der Berechtigungen für jede integrierte Rolle finden Sie unter ["Integrierte Rollen für Azure-Ressourcen"](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Sie verfügen nicht über die Berechtigung zum Erstellen einer Supportanfrage**: Wenn Sie versuchen, ein Supportticket zu erstellen oder zu aktualisieren, überprüfen Sie, ob Sie derzeit mit einem Benutzer angemeldet sind, dem eine Rolle mit der Berechtigung "Microsoft.Support/supportTickets/write" zugewiesen ist, z. B. [Mitwirkender für Supportanfragen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Es können keine weiteren Rollenzuweisungen erstellt werden (Code: RoleAssignmentLimitExceeded):** Wenn Sie versuchen, eine Rolle zuzuweisen, versuchen Sie, die Anzahl der Rollenzuweisungen zu reduzieren, indem Sie stattdessen Gruppen Rollen zuweisen. Azure unterstützt bis zu **2.000** Rollenzuweisungen pro Abonnement.

Weitere Informationen zu Azure RBAC-Rollen finden Sie unter [Azure RBAC-Rollen](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
