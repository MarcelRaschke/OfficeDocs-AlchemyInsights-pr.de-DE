---
title: Probleme beim Verwenden der Intune-Verwaltungskonsole
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000214"
- "1790"
ms.date: 07/29/2020
ms.openlocfilehash: 0019d8258ec63302f824dbc98e5c2f845291d1ef
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66386841"
---
# <a name="problems-using-the-intune-admin-console"></a>Probleme beim Verwenden der Intune-Verwaltungskonsole

**"Zugriff verweigert" beim Navigieren im Intune-Verwaltungsportal.**

- Wenn Sie Mitglied einer benutzerdefinierten Intune-Rolle sind, stellen Sie sicher, dass Ihrem Konto eine Intune- oder Enterprise Mobility Suite-Lizenz zugewiesen ist.
- Wenn Sie Configuration Manager zum Verwalten von Geräten verwenden, stellen Sie sicher, dass Sie nicht zur Intune-Benutzersammlung für Configuration Manager-MDM gehören.
- Stellen Sie sicher, dass Ihnen im Blatt"Intune-Rolle" die entsprechenden RBAC-Berechtigungen (rollenbasierte Zugriffssteuerung) zugewiesen wurden.
- Vergewissern Sie sich, dass die verwendete Gruppe keine Verteilerliste ist. Intune im Azure-Portal unterstützt nur Benutzerkonten, die zu Azure Active Directory-Sicherheitsgruppen gehören. Überprüfen Sie Ihre Gruppen unter Azure-Portal > **Intune** > **Gruppen**, oder unter Azure-Portal > **Azure Active Directory**.

**Der Benutzer verfügt über zu viele Berechtigungen für die zugewiesene Intune-Rolle**

Weisen Sie den Benutzer an, zu **Intune** > **Intune-Rollen** > **Meine Berechtigungen** > **Exportieren** zu wechseln, um die gewährten Berechtigungen zu überprüfen.

**Ich habe eine Bereichsgruppe zu einer Rolle hinzugefügt, aber die Benutzer in dieser Rolle sehen weiterhin andere Benutzer oder Geräte.**

Bereichsgruppen filtern keine Benutzer oder Geräte heraus. Bereichsgruppen tun Folgendes:

- Beschränken, web Benutzer Richtlinien oder Anwendungen zuordnen können.
- Erlauben nur bestimmten Benutzern das Ausführen von Remoteaufgaben auf Geräten.

Weitere Informationen über Bereichsgruppen finden Sie unter [Rollenbasierte Zugriffssteuerung (RBAC) mit Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Ich habe einen Benutzer zu einer Intune-Rolle hinzugefügt, aber er hat immer noch vollen Zugriff auf die Intune-Verwaltungskonsole.**

Navigieren Sie im Azure-Portal zu Intune > **Benutzer** dem Benutzer keine der folgenden Rollen im Azure-Portal zugewiesen ist:

- Globaler Administrator
- Intune-Dienstadministrator
- SharePoint-Administrator

Weitere Informationen finden Sie unter [Rollenbasierte Zugriffssteuerung (RBAC) mit Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Access-Probleme**

Weitere Informationen finden Sie unter [Anmelden bei Office 365, Azure oder Intune nicht möglich](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).