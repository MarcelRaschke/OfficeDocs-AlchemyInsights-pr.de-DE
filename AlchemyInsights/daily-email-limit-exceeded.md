---
title: Das tägliche E-Mail-Limit wurde überschritten. Der Workflow wird angehalten.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 2f18c1be46c528b957f16f10a86d60950ce1f668
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63204764"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Tägliche E-Mail-Grenze überschritten. Der Workflow wird angehalten.

Dieser Fehler kann in den folgenden Szenarien empfangen werden:

- Sie verfügen über einen Workflow in SharePoint Online, der den Workflowplattformtyp SharePoint 2010 oder SharePoint 2013 verwendet.
- Der Workflow ist so konfiguriert, dass eine benutzerdefinierte E-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute gesendet wird.
- Wenn Sie den Workflow ausführen, wird die E-Mail-Nachricht nicht gesendet, und Sie bemerken das folgende Verhalten:
    - Für einen Workflow, der den Plattformtyp SharePoint 2013 verwendet, navigieren Sie zur Seite **"Workflowstatus**". Auf der Seite "Workflowstatus" ist der **interne Status** auf **"Gestartet**" festgelegt, und in der Informationssprechblase wird angezeigt, dass **das Senden an einen Empfänger nicht möglich** ist.

Um dieses Problem zu umgehen, konfigurieren Sie Ihren Workflow so, dass E-Mail-Nachrichten gesendet werden, ohne die [Grenzwerte für Exchange Online Absender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) zu überschreiten. Verwenden Sie beispielsweise eine Pause im Workflow, senden Sie die E-Mail an eine Microsoft 365 Gruppe, eine Verteilergruppe oder eine E-Mail-aktivierte Sicherheitsgruppe, oder senden Sie die Nachricht an weniger als 200 Empfänger gleichzeitig.


Weitere Informationen finden Sie im folgenden [Artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Verwandte Themen
- [Erstellen Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 