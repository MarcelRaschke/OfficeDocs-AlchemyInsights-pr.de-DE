---
title: Das tägliche E-Mail-Limit wurde überschritten. Der Workflow wird angehalten.
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
- "1227"
ms.openlocfilehash: b460d558f572b137eb6be240798dc509bb3a9f13
ms.sourcegitcommit: 8324c868c664bfdee6d5bb99ad8d41e9dd46d10f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66539162"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Das tägliche E-Mail-Limit wurde überschritten. Der Workflow wird angehalten.

Dieser Fehler kann in den folgenden Szenarien auftreten:

- Sie haben einen Workflow in SharePoint Online, der den SharePoint 2010- oder SharePoint 2013-Workflowplattformtyp verwendet.
- Der Workflow ist so konfiguriert, dass eine benutzerdefinierte E-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute gesendet wird.
- Wenn Sie den Workflow ausführen, wird die E-Mail-Nachricht nicht gesendet, und Sie bemerken das folgende Verhalten:
    - Für einen Workflow mit dem SharePoint 2013-Plattformtyp navigieren Sie zur Seite **"Workflowstatus** ". Auf der Seite "Workflowstatus" ist der **interne Status** auf " **Gestartet**" festgelegt, und die Informationssprechblase zeigt " **Nicht senden an einen Empfänger" an**.

Um dieses Problem zu umgehen, konfigurieren Sie Ihren Workflow so, dass E-Mail-Nachrichten gesendet werden, ohne die [Grenzwerte für Exchange Online Absender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) zu überschreiten. Verwenden Sie beispielsweise eine Pause im Workflow, senden Sie die E-Mail an eine Microsoft 365-Gruppe, eine Verteilergruppe oder eine E-Mail-aktivierte Sicherheitsgruppe, oder senden Sie die Nachricht an weniger als 200 Empfänger gleichzeitig.


Weitere Informationen finden Sie im folgenden [Artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Verwandte Themen
- [Fluss erstellen](https://support.microsoft.com/office/create-a-flow-for-a-list-or-library-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 