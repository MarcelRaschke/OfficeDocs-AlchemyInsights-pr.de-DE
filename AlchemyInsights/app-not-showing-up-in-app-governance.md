---
title: Meine App wird nicht in app Governance angezeigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362393"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Meine App wird nicht in app Governance angezeigt

Wenn Ihre Anwendung nicht in der App-Governance angezeigt wird, überprüfen Sie Folgendes:

1. Wechseln Sie zu [Azure AD,](https://aad.portal.azure.com/) und suchen Sie die App-ID für Ihre Anwendung, indem Sie in der oberen Leiste auf der Übersichtsseite nach dem App-Namen suchen.

1. Greifen Sie auf Graph Explorer zu, und suchen Sie innerhalb Ihres Dienstprinzipals nach der App-ID, indem Sie diese Abfrage verwenden und <appId> durch die entsprechende App-ID ersetzen: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Wenn keine Ergebnisse zurückgegeben werden, suchen Sie mit dieser Abfrage nach der App-ID innerhalb der Anwendung, und ersetzen Sie sie <appId> durch die entsprechende App-ID: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Wenn Probleme mit der Abfrage auftreten, finden Sie weitere Informationen unter ["Support erhalten".](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Weitere Informationen oder Einblicke in Ihre Apps in App Governance finden Sie unter ["Informationen zu Sichtbarkeit und Einblicken".](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Weitere Informationen zum Anzeigen Ihrer Apps finden Sie unter [Anzeigen Ihrer Apps.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
