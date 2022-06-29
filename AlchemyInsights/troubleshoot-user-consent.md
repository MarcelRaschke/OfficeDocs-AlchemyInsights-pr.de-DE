---
title: Problembehandlung bei der Zustimmung des Benutzers
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004353"
- "7785"
ms.date: 01/18/2021
ms.openlocfilehash: 4194743d4ecd8fe95cc925c0f8ca78f826e32bbf
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66371127"
---
# <a name="troubleshoot-user-consent"></a>Problembehandlung bei der Zustimmung des Benutzers

1. Sie können konfigurieren, wie Endbenutzer Anwendungen über das Azure-Portal oder PowerShell zustimmen. Weitere Informationen finden Sie unter ["Benutzer-Zustimmungseinstellungen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) ".
1. Ein Administrator kann die [Microsoft Graph-API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) auch verwenden, um delegierten Berechtigungen im Namen eines einzelnen Benutzers zuzustimmen. Weitere Informationen finden Sie unter ["Zugriff im Namen eines Benutzers erhalten"](https://docs.microsoft.com/graph/auth-v2-user).
1. [Fehler bei der Benutzerzustimmung](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): In diesem Artikel werden Fehler erläutert, die während der Zustimmung zu einer Anwendung auftreten können. Wenn Sie unerwartete Zustimmungsaufforderungen behandeln, die keine Fehlermeldungen enthalten, lesen Sie [Authentifizierungsszenarien für Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).