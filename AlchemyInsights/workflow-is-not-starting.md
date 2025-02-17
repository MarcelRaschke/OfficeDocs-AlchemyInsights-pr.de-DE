---
title: Workflow wird nicht gestartet
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
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794766"
---
# <a name="workflow-is-not-starting"></a>Workflow wird nicht gestartet

- SharePoint 2010-und SharePoint 2013-Workflows werden nicht gestartet.

    - Wenn Ihr Workflow nicht gestartet wird, kann es zu einem temporären Dienst Problem kommen, bei dem Benutzer gelegentlich Verzögerungen mit dem Workflowfortschritt auftreten können. Überprüfen Sie das [Dienststatus-Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , um zu sehen, ob Ihre Organisation betroffen ist.

    - Wenn seit dem ersten Auftreten dieses Problems mehr als 24 Stunden vergangen sind, melden Sie sich ein Support Ticket an. In vielen Fällen arbeiten wir bereits an einer Lösung. Geben Sie uns mindestens 24 Stunden, um eine Lösung zu vervollständigen.

- SharePoint 2010-Workflows werden beim Start verzögert.

    - Dies tritt auf, wenn der Workflow in großen Batches ausgelöst wird. (beispielsweise, wenn mehrere Elemente gleichzeitig hinzugefügt werden).

    - Workflows sind nicht für die Ausführung in Echtzeit vorgesehen, daher ist eine Verzögerung das Entwurfsverhalten.

   -  Wenn es sich bei dem Workflow um eine komplexe eXtensible Object Markup Language (XMol) handelt, kann die Kompilierung langsam sein. Lesen Sie [diesen](https://support.microsoft.com//kb/3043697) Artikel.

    - Sie sollten den Workflow vereinfachen oder ihn mit dem Microsoft SharePoint 2013 Workflow Platt Form neu entwerfen.

    - Wenn Ihr Workflowverlauf groß geworden ist, können Sie die Elemente löschen oder eine neue Verlaufsliste erstellen.

        Weitere Informationen: [Workflow Verlauf löschen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Fluss erstellen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


