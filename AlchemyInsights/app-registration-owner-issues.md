---
title: Probleme mit dem Besitzer der App-Registrierung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951132"
---
# <a name="app-registration-owner-issues"></a>Probleme mit dem Besitzer der App-Registrierung

Es folgen die verfügbaren Methoden zum Hinzufügen von Prinzipalen als Besitzer für App-Registrierungen:

- Verwenden des Azure AD PowerShell-Moduls –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referenz: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Verwenden von Azure CLI – `az ad app owner add`

    Referenz: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Verwenden von MS-Graph –

    Referenz: [Besitzer hinzufügen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Verwenden des Azure AD-Portals – Navigieren Sie zu [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App-Registrierung > Wählen Sie Ihre Anwendung aus, > Besitzer > Besitzer hinzufügen

**Können Sie Ihre Anwendung nicht auf dem Blatt "App-Registrierungen" anzeigen, obwohl Sie der Besitzer dieser Anwendung sind?**

Der Besitzer einer App ist keine Administratorrolle. Wenn die Einstellung ["Zugriff auf Azure AD-Verwaltungsportal einschränken"](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) aktiviert ist, kann nur der Administrator die Anwendungen im App-Registrierungsportal anzeigen. Damit ein Besitzer die Anwendungen anzeigen kann, deaktivieren Sie diese Einstellung (Legen Sie diese auf NEIN fest), oder weisen Sie dem Besitzer nur für die jeweilige Anwendung eine Administratorrolle zu. Hierfür benötigen Sie jedoch eine Azure AD Premium P2-Lizenz und aktivieren [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
