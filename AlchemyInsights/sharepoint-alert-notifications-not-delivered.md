---
title: SharePoint nicht zugestellte Benachrichtigungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 2ac6d48043f02f2626ba02863044f133207c0ba5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63157711"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint nicht zugestellte Benachrichtigungen

Überprüfen Sie den JUNK-Ordner in Ihrer E-Mail, da manchmal Warnungen hingehen können.

Ermitteln Sie, ob **nicht alle Warnungen übermittelt werden** oder ob **eine einzelne Warnung** aus einer bestimmten Datei oder Bibliothek nicht übermittelt wird.

- **Einzelne Warnungen werden nicht übermittelt**: Wenn eine einzelne Warnung aus einer bestimmten Datei oder Bibliothek nicht übermittelt wird, können Sie versuchen, sie zu löschen und neu zu erstellen. Weitere Informationen finden Sie unter [Verwalten, Anzeigen oder Löschen SharePoint Warnungen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2), um die Warnung neu zu erstellen.
- **Alle Warnungen werden nicht übermittelt**: Wenn alle Warnungen aus mehreren Dateien oder Bibliotheken nicht übermittelt werden, besuchen Sie das [Dienststatus-Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth), um nach Empfehlungen/Vorfällen zu suchen, die bei SharePoint oder Exchange auftreten können. Das Problem kann mit der SharePoint Benachrichtigungsfunktion oder Verzögerungen in E-Mails über Exchange auftreten. Es ist auch wichtig zu beachten, ob andere E-Mails zugestellt werden, und wenn nicht, ist das Problem wahrscheinlich mit Exchange Verzögerungen verbunden.

Häufig gestellte Fragen zu Warnungen:

- Es ist nicht möglich, Warnungen an Verteilergruppen zu senden, nur Sicherheits- und O365-Gruppen werden unterstützt.
- E-Mail-Vorlagen für Warnungen können nicht angepasst werden. Sie müssen Microsoft FLOW oder SharePoint Designer-Workflow verwenden, um dies zu erreichen.

## <a name="related-topics"></a>Verwandte Themen

Möchten Sie Microsoft Flow in SharePoint Online testen?

- [Erstellen Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint und Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
