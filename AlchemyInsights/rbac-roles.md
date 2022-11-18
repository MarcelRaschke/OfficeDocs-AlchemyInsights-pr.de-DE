---
title: 'RBAC-Rollen '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 06bab4e5a5ca4b24fee33dae603850a96af7ff40
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66400035"
---
# <a name="rbac-rules"></a>RBAC-Regeln

Wenn der Berechtigungsfehler angezeigt wird: 

- **Der Client mit Objekt-ID verfügt nicht über die Autorisierung zum Ausführen einer Aktion über den Bereich (Code: AuthorizationFailed):** Wenn Sie versuchen, eine Ressource zu erstellen, überprüfen Sie, ob Sie derzeit bei einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, die über Schreibberechtigungen für die Ressource im ausgewählten Bereich verfügt. Um beispielsweise virtuelle Computer in einer Ressourcengruppe zu verwalten, sollten Sie die Rolle " [Mitwirkender für virtuelle Computer](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) " in der Ressourcengruppe (oder im übergeordneten Bereich) haben. Eine Liste der Berechtigungen für jede integrierte Rolle finden Sie [unter Integrierte Rollen für Azure-Ressourcen](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Sie verfügen nicht über die Berechtigung zum Erstellen einer Supportanfrage**: Wenn Sie versuchen, ein Supportticket zu erstellen oder zu aktualisieren, überprüfen Sie, ob Sie derzeit bei einem Benutzer angemeldet sind, dem eine Rolle zugewiesen ist, der die Berechtigung "Microsoft.Support/supportTickets/write" zugewiesen ist, z. B. ["Mitwirkender für Supportanfrage](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)".
- **Es können keine weiteren Rollenzuweisungen erstellt werden (Code: RoleAssignmentLimitExceeded)**: Wenn Sie versuchen, eine Rolle zuzuweisen, versuchen Sie, die Anzahl der Rollenzuweisungen zu verringern, indem Sie stattdessen Gruppen Rollen zuweisen. Azure unterstützt bis zu **2000** Rollenzuweisungen pro Abonnement.

Weitere Informationen zu Azure RBAC-Rollen finden Sie unter [Azure RBAC-Rollen](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
