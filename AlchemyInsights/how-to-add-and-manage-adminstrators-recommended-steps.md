---
title: Hinzufügen und Verwalten von Administratoren – empfohlene Schritte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: b6e4afb4b96d7644e5989f05b21028be5ca1bd6d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63256445"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Hinzufügen und Verwalten von Administratoren – empfohlene Schritte

Basierend auf Ihrer Problembeschreibung haben wir eine Lösung für Sie gefunden. Die meisten Kunden konnten ihr Problem selbst beheben, nachdem sie unserer Dokumentation folgten.

**Bearbeiten des Abonnementadministrators oder Co-Administrators**

- Der Kontoadministrator kann beide Rollen bearbeiten, während der Abonnementadministrator nur Co-Administratoren im [Azure-Portal](https://ms.portal.azure.com/#home) ändern kann.
- [Hinzufügen oder Ändern von Azure-Abonnementadministratoren](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Aktualisieren des Abonnementadministrators oder Co-Administrator für interne Abonnements (AIRS)**

Der Dienstadministrator oder der Co-Administrator kann diese Aktion mithilfe der folgenden Schritte selbst ausführen:

1. Melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) an, und klicken Sie auf dem linken Blatt auf **"Kostenverwaltung + Abrechnung** ".
2. Klicken Sie auf die Zeile mit Ihrem Abonnement. Dadurch wird die Übersicht für Ihr Abonnement geöffnet.
3. Klicken Sie auf dem Blatt **"Abonnement** " auf **"Eigenschaften**". 
4. Klicken Sie auf die Schaltfläche " **Dienstadministrator** ".
5. Geben Sie die E-Mail des Benutzers ein, den Sie als Dienstadministrator festlegen möchten, und klicken Sie auf **"OK**".

**Hinzufügen/Ändern/Entfernen des Co-Administrators**

1. Melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) als Dienstadministrator an.
2. Öffnen [Sie Abonnements](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , und wählen Sie ein Abonnement aus. (Mitadministratoren können nur im Abonnementbereich zugewiesen werden.)
3. Navigieren Sie zu **Access Control (IAM)** > **Classic** **administratorsAddAdd** >  >  **co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).
4. Wählen Sie den Benutzer aus, den Sie hinzufügen möchten, und klicken Sie auf **"Hinzufügen**".

**Weitere Informationen:**
- [Hinzufügen eines Co-Administrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Entfernen eines Co-Administrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ändern des Dienstadministrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Anzeigen des Kontoadministrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Verwalten des Zugriffs mithilfe von RBAC und dem Azure-Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Hinzufügen/Löschen von Benutzern mit Azure Active Directory (AD)**

Sie können neue Benutzer hinzufügen oder vorhandene Benutzer aus Ihrer Azure Active Directory (Azure AD) Organisation löschen:

1. Um einen neuen Benutzer hinzuzufügen, melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) als Benutzeradministrator für die Organisation an.
2. Wählen Sie **Azure Active Directory** aus, wählen Sie **"Benutzer"** aus, und klicken Sie dann auf **"Neuer Benutzer**".
3. Geben Sie auf der **Seite "Benutzer** " die erforderlichen Informationen ein. Klicken Sie auf **Erstellen**. Der Benutzer wird erstellt und Ihrem Azure AD Mandanten hinzugefügt.

**Weitere Informationen**:

- [Hinzufügen eines neuen Benutzers](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Benutzer löschen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Hinzufügen oder Aktualisieren der Profilinformationen eines Benutzers mithilfe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Empfohlene Dokumente**

- [Was ist die rollenbasierte Zugriffssteuerung (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Grundlegendes zu den verschiedenen Rollen in Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratorrollenberechtigungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Lernprogramm: Gewähren des Zugriffs für einen Benutzer mithilfe von RBAC und dem Azure-Portal](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Problembehandlung bei RBAC in Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organisieren Ihrer Ressourcen mit Azure-Verwaltungsgruppen](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Anfordern einer Kopie der Azure-Rechnung per E-Mail](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Hinzufügen, Aktualisieren oder Entfernen einer Kredit- oder Debitkarte aus Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Verwalten (Reaktivieren/Kündigen/Wechseln) eines Abonnements](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



