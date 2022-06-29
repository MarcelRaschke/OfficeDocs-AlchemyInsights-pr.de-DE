---
title: Zugriffsüberprüfungen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004349"
- "7767"
ms.date: 01/27/2021
ms.openlocfilehash: 29c5a74c313eee0ddbc12b1cb4dad12522cd723d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66314499"
---
# <a name="access-reviews"></a>Zugriffsüberprüfungen

1. **Aktivieren von Zugriffsüberprüfungen**: Sie können Rezensionen aktivieren, wenn Sie ein neues Zugriffspaket erstellen oder ein vorhandenes Zugriffspaket bearbeiten. [Das Erstellen einer Zugriffsüberprüfung eines Zugriffspakets in der Azure AD-Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) beschreibt, wie Zugriffsüberprüfungen von Zugriffspaketen aktiviert werden.

1. **Überprüfen von Zugriff**: Die Verwaltung von Azure AD-Berechtigungen vereinfacht die Verwaltung des Zugriffs auf Gruppen, Anwendungen und SharePoint-Websites durch Unternehmen. [Der Zugriff auf ein Zugriffspaket in der Azure AD-Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) wird beschrieben, wie Zugriffsüberprüfungen für andere Benutzer ausgeführt werden, die einem Zugriffspaket als festgelegter Prüfer zugewiesen sind.

1. **Überprüfen von Access für sich selbst**: [Die Selbstüberprüfung eines Zugriffspakets in der Azure AD-Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) beschreibt, wie ein Benutzer seine zugewiesenen Zugriffspakete selbst überprüft.

1. In den meisten Fällen finden Endbenutzer eine Überprüfung, bis ihre Antwort in der **Zugriffsbereich**. Dies gilt nur für Rezensionen von Gruppen und Anwendungen, nicht für Rollen. Für alle Zugriffsüberprüfungen von Rollen müssen Endbenutzer zu Azure AD Privileged Identity Management (PIM) navigieren, um ihre Überprüfung abzuschließen.

    1. Melden Sie sich beim Azure-Portal an.
    2. Navigieren Sie zu Azure AD PIM.
    3. Wählen Sie im linken Navigationsbereich den Zugriff auf **"Aufgabenüberprüfung** > **"** aus.
    
Weitere Informationen finden Sie unter:

- [Durchführen einer Zugriffsüberprüfung meiner Azure AD-Verzeichnisrollen in PIM ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [Durchführen einer Zugriffsüberprüfung meiner Azure-Ressourcenrollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)