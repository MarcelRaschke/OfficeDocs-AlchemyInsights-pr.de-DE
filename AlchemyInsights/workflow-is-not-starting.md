---
title: Der Workflow wird nicht gestartet.
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000144"
- "1670"
ms.date: 04/21/2020
ms.openlocfilehash: d13b2a45f4af5a2f31c4b4fba9935f036c1dd624
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66587551"
---
# <a name="workflow-is-not-starting"></a>Der Workflow wird nicht gestartet.

- SharePoint 2010- und SharePoint 2013-Workflows werden nicht gestartet.

    - Wenn Ihr Workflow nicht gestartet wird, kann es zu einem temporären Dienstproblem kommen, bei dem Benutzer mit dem Workflowfortschritt zeitweilige Verzögerungen feststellen können. Überprüfen Sie das [Dienstintegritätsdashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) , um festzustellen, ob Ihre Organisation betroffen ist.

    - Wenn mehr als 24 Stunden vergangen sind, seit Sie dieses Problem zum ersten Mal gesehen haben, melden Sie sich bitte ein Supportticket an. In vielen Fällen arbeiten wir bereits an einer Lösung. Bitte geben Sie uns mindestens 24 Stunden, um eine Lösung abzuschließen.

- SharePoint 2010-Workflows beim Start verzögert.

    - Dies tritt auf, wenn der Workflow in großen Batches ausgelöst wird. (z. B. wenn mehrere Elemente gleichzeitig hinzugefügt werden).

    - Workflows sind nicht für die Ausführung in Echtzeit ausgelegt, daher ist eine Verzögerung designbedingtes Verhalten.

   -  Wenn der Workflow komplex XMOL (Extensible Object Markup Language) ist, kann die Kompilierung langsam sein. Lesen Sie [diesen](https://support.microsoft.com//kb/3043697) Artikel.

    - Sie sollten den Workflow vereinfachen oder mithilfe des Microsoft SharePoint 2013-Workflowplattformtyps neu entwerfen.

    - Wenn Ihr Workflowverlauf groß geworden ist, können Sie die Elemente löschen oder eine neue Verlaufsliste erstellen.

        Weitere Informationen: [Löschen des Workflowverlaufs](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Fluss erstellen](https://support.microsoft.com/office/create-a-flow-for-a-list-or-library-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
