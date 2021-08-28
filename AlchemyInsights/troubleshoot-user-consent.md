---
title: Problembehandlung bei der Zustimmung des Benutzers
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007897"
---
# <a name="troubleshoot-user-consent"></a>Problembehandlung bei der Zustimmung des Benutzers

1. Sie können konfigurieren, wie Endbenutzer Anwendungen über das Azure-Portal oder PowerShell zustimmen. Weitere Informationen finden Sie in den Einstellungen für [die Benutzergenehmigung.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)
1. Ein Administrator kann auch die [Microsoft Graph-API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) verwenden, um delegierte Berechtigungen im Namen eines einzelnen Benutzers zu erteilen. Weitere Informationen finden Sie unter ["Zugriff im Namen eines Benutzers erhalten".](https://docs.microsoft.com/graph/auth-v2-user)
1. [Benutzerzustimmungsfehler:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)In diesem Artikel werden Fehler behandelt, die während des Prozesses der Zustimmung zu einer Anwendung auftreten können. Wenn Sie unerwartete Zustimmungsaufforderungen, die keine Fehlermeldungen enthalten, behandeln, lesen Sie die [Authentifizierungsszenarien für Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)