---
title: Zugriffsüberprüfungen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: 8925894c3efb3ae19deba01746c89eda793249dd
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63288557"
---
# <a name="access-reviews"></a>Zugriffsüberprüfungen

1. **Aktivieren von Zugriffsüberprüfungen**: Sie können Rezensionen aktivieren, wenn Sie ein neues Zugriffspaket erstellen oder ein vorhandenes Zugriffspaket bearbeiten. [Erstellen einer Zugriffsüberprüfung eines Zugriffspakets in Azure AD Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) beschreibt, wie Zugriffsüberprüfungen von Zugriffspaketen aktiviert werden.

1. **Überprüfen des Zugriffs**: Azure AD Berechtigungsverwaltung vereinfacht, wie Unternehmen den Zugriff auf Gruppen, Anwendungen und SharePoint Websites verwalten. [Überprüfen des Zugriffs auf ein Zugriffspaket in Azure AD Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) beschreibt, wie Zugriffsüberprüfungen für andere Benutzer durchgeführt werden, die einem Zugriffspaket als festgelegter Prüfer zugewiesen sind.

1. **Überprüfen des Zugriffs für sich selbst**: [Die Selbstüberprüfung eines Zugriffspakets in Azure AD Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) beschreibt, wie ein Benutzer seine zugewiesenen Zugriffspakete selbst überprüft.

1. In den meisten Fällen finden Endbenutzer eine Rezension, bis ihre Antwort im **Zugriffsbereich** aussteht. Dies gilt nur für Rezensionen von Gruppen und Anwendungen, nicht für Rollen. Für alle Zugriffsüberprüfungen von Rollen müssen Endbenutzer zu Azure AD Privileged Identity Management (PIM) navigieren, um ihre Rezension abzuschließen.

    1. Melden Sie sich beim Azure-Portal an.
    2. Navigieren Sie zu Azure AD PIM.
    3. Wählen Sie im linken Navigationsbereich **"****TasksReview** >  Access" aus.
    
Weitere Informationen finden Sie unter:

- [Durchführen einer Zugriffsüberprüfung meiner Azure AD Verzeichnisrollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [Durchführen einer Zugriffsüberprüfung meiner Azure-Ressourcenrollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)