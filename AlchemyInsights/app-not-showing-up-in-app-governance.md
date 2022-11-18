---
title: Meine App wird in der App-Governance nicht angezeigt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9007647"
- "12734"
ms.date: 8/16/2021
ms.openlocfilehash: 8053b54d86cc2893f4b265603ca82f3530ef9c27
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66300664"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Meine App wird in der App-Governance nicht angezeigt

Wenn Ihre Anwendung nicht in der App-Governance angezeigt wird, überprüfen Sie Folgendes:

1. Wechseln Sie zu [Azure AD](https://aad.portal.azure.com/) , und suchen Sie die App-ID für Ihre Anwendung, indem Sie in der oberen Leiste auf der Seite "Übersicht" nach dem App-Namen suchen.

1. Greifen Sie auf den Graph-Explorer zu, und suchen Sie nach der App-ID in Ihrem Dienstprinzipal, indem Sie diese Abfrage verwenden und durch die entsprechende App-ID ersetzen \<appId\> :  `<https://graph.microsoft.com/v1.0/servicePrincipals?$search="appId:<appId>">`

1. Wenn keine Ergebnisse zurückgegeben werden, suchen Sie mithilfe dieser Abfrage nach der App-ID in der Anwendung, und ersetzen Sie \<appId\> sie durch die entsprechende App-ID:  `<https://graph.microsoft.com/v1.0/applications?$search= "appId:<appId>">`

Wenn Probleme mit der Abfrage auftreten, lesen [Sie "Support anfordern"](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Weitere Informationen oder Einblicke in Ihre Apps in App-Governance finden [Sie unter "Informationen zu Sichtbarkeit und Einblicken](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)".

Weitere Informationen zum Anzeigen Ihrer Apps finden Sie unter ["Anzeigen Ihrer Apps](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)".
