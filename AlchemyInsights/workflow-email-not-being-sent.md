---
title: Workflow-E-Mails werden nicht gesendet
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "5200020"
- "1586"
ms.date: 04/21/2020
ms.openlocfilehash: 6d1fed5d8dba5f47a0869c961902386bd5f04272
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66527088"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Workflow-E-Mails werden nicht für eine SharePoint-Liste oder -Bibliothek gesendet.

1. E-Mails von Workflows werden nicht an alle Benutzer oder nur an bestimmte Benutzer gesendet, oder es wird der Fehler angezeigt **. Die E-Mail-Nachricht kann nicht gesendet werden. Stellen Sie sicher, dass die E-Mail über einen gültigen Empfänger verfügt**.

    Überprüfen Sie, ob der Benutzer in der Berechtigungsgruppe " **Alle Personen** " (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.  Beispiel für eine direkte URL: https://\<tenant\>.sharepoint.com/sites/\<sitename\>/_layouts/15/people.aspx? MembershipGroupId=0

    - Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist. 
    - Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass seine Einladung angenommen wurde.
    - Wenn der Benutzer in der Berechtigungsgruppe vorhanden ist, stellen Sie sicher, dass die E-Mail-Adresse korrekt ist.
    - Wenn die E-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielbenachrichtigung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos aus Benutzerprofilen von SharePoint mit dieser Websitesammlung erzwingt.
 
2. E-Mails von Workflows werden an die Websitesammlungsadministratoren, aber nicht an andere Benutzer gesendet und sehen den Fehler **HTTP Forbidden to <span>https:</span>://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Siehe ["Zugriff verweigert", wenn Sie eine E-Mail an eine SharePoint-Gruppe senden](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Stellen Sie außerdem sicher, dass die Websitesammlungsfunktion für den **Sperrmodus für Benutzerberechtigungen mit eingeschränktem Zugriff** nicht aktiv ist.


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Fluss erstellen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


