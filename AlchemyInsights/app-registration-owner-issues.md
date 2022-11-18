---
title: Probleme mit dem App-Registrierungsbesitzer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 080860ca2b378de26ffc4199f3eb96ebfb1bb15a
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66275140"
---
# <a name="app-registration-owner-issues"></a>Probleme mit dem App-Registrierungsbesitzer

Es folgen die verfügbaren Methoden zum Hinzufügen von Prinzipalen als Besitzer für App-Registrierungen:

- Verwenden des Azure AD PowerShell-Moduls –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referenz: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Verwenden von Azure CLI – `az ad app owner add`

    Referenz: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Verwenden von MS Graph -

    Referenz: [Besitzer hinzufügen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Verwenden des Azure AD-Portals – Navigieren Sie zu [portal.azure.com >](https://portal.azure.com/) Azure Active Directory > App-Registrierung > Wählen Sie Ihre Anwendung > Besitzer aus, > Besitzer hinzufügen

**Sie können Ihre Anwendung nicht auf dem Blatt "App-Registrierungen" anzeigen, obwohl Sie der Besitzer dieser Anwendung sind?**

Der Besitzer einer App ist keine administrative Rolle. Wenn die Einstellung ["Zugriff auf Das Azure AD-Verwaltungsportal einschränken](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) " aktiviert ist, können nur Administratoren die Anwendungen im App-Registrierungsportal anzeigen. Damit ein Besitzer die Anwendungen anzeigen kann, deaktivieren Sie entweder diese Einstellung (legen Sie diese auf NEIN fest) oder weisen Sie dem Besitzer nur die Administratorrolle für die bestimmte Anwendung zu. Dafür benötigen Sie jedoch eine Azure AD Premium P2 Lizenz und aktivieren [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
