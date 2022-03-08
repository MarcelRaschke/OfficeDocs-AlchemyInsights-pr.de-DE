---
title: Meine App wird nicht in app Governance angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: 8c95c4a53d9ea9f9610b854b4f0c98439dc09d96
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63279413"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Meine App wird nicht in app Governance angezeigt

Wenn Ihre Anwendung nicht in der App-Governance angezeigt wird, überprüfen Sie Folgendes:

1. Wechseln Sie zu [Azure AD](https://aad.portal.azure.com/), und suchen Sie die App-ID für Ihre Anwendung, indem Sie in der oberen Leiste auf der Übersichtsseite nach dem App-Namen suchen.

1. Greifen Sie auf Graph Explorer zu, und suchen Sie in Ihrem Dienstprinzipal nach der App-ID, indem Sie diese Abfrage verwenden und durch die entsprechende App-ID ersetzen\<appId\>:`<https://graph.microsoft.com/v1.0/servicePrincipals?$search="appId:<appId>">`

1. Wenn keine Ergebnisse zurückgegeben werden, suchen Sie mithilfe dieser Abfrage nach der App-ID in der Anwendung und ersetzen Sie \<appId\> sie durch die entsprechende App-ID:  `<https://graph.microsoft.com/v1.0/applications?$search= "appId:<appId>">`

Wenn Probleme mit der Abfrage auftreten, lesen [Sie "Support anfordern](https://docs.microsoft.com/microsoft-365/business-video/get-help-support)". 

Weitere Informationen oder Einblicke in Ihre Apps in App Governance finden Sie unter ["Informationen zu Sichtbarkeit und Einblicken](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)".

Weitere Informationen zum Anzeigen Ihrer Apps finden Sie unter ["Anzeigen Ihrer Apps](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)".
