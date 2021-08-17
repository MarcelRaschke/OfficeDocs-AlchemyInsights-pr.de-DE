---
title: Workflow-E-Mail wird nicht gesendet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072519"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Workflow-E-Mails werden nicht für eine SharePoint Liste oder Bibliothek gesendet

1. E-Mails von Workflows werden nicht an alle Benutzer oder nur bestimmte Benutzer gesendet, oder es wird der Fehler **angezeigt. Die E-Mail-Nachricht kann nicht gesendet werden. Stellen Sie sicher, dass die E-Mail einen gültigen Empfänger hat.**

    Überprüfen Sie, ob der Benutzer in der Berechtigungsgruppe **"Alle Personen"** (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.  Direkte Beispiel-URL: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist. 
    - Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass die Einladung angenommen wurde.
    - Wenn der Benutzer in der Berechtigungsgruppe vorhanden ist, stellen Sie sicher, dass die E-Mail-Adresse korrekt ist.
    - Wenn die E-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielwarnung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos von Benutzerprofilen von SharePoint zu dieser Websitesammlung erzwingt.
 
2. E-Mails von Workflows werden an die Websitesammlungsadministratoren, aber nicht an andere Benutzer gesendet und der Fehler **HTTP Forbidden to <span>https:</span>://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail** angezeigt.
 

    Siehe ["Zugriff verweigert", wenn Sie eine E-Mail an eine SharePoint Gruppe senden.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Stellen Sie außerdem sicher, dass die Websitesammlungsfunktion für den Sperrmodus für **Benutzerberechtigungen** mit eingeschränktem Zugriff nicht aktiv ist.


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Erstellen Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


