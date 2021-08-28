---
title: Zuweisen einer Überwachungsprotokoll-Rolle im Office 365 Security & Compliance Center
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 5ddfda8687fe3ae2467ad221c7c083f46239826e23b10b91732ea06fd4649f3e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54006169"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Zuweisen einer Überwachungsprotokoll-Rolle im Office 365 Security & Compliance Center

Einem Administrator muss in Exchange Online entweder die Rolle **Überwachungsprotokolle nur anzeigen** oder die Rolle **Überwachungsprotokolle** zugewiesen werden, damit er das Office 365-Überwachungsprotokoll durchsuchen kann. Standardmäßig sind diese Rollen den Rollengruppen „Complianceverwaltung“ und „Organisationsverwaltung“ zugewiesen. Globale Administratoren in Office 365 und Microsoft 365 sind automatisch Mitglieder der Rollengruppe „Organisationsverwaltung“.

Damit ein Benutzer das Überwachungsprotokoll mit minimalen Rechten durchsuchen kann, erstellen Sie in Exchange Online eine benutzerdefinierte Rollengruppe, fügen ihr die Rolle **Überwachungsprotokolle nur anzeigen** oder die Rolle **Überwachungsprotokolle** hinzu und fügen den Benutzer dann als Mitglied der neuen Rollengruppe hinzu.

Weitere Informationen finden Sie unter [Verwalten von Rollengruppen in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) und [Durchsuchen des Überwachungsprotokolls im Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).