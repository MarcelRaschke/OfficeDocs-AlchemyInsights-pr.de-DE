---
title: Fehler beim Aktivieren des fehlenden Workflows
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: eef6162f2d0659d18ef2aa23fa0a4e3aa6a1717e
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65725441"
---
# <a name="missing-workflow-failed-to-activate"></a>Fehler beim Aktivieren des fehlenden Workflows

In einer Microsoft SharePoint-Websitesammlung können Sie zu einer Liste oder Bibliothek keinen global wiederverwendbaren Workflow (z. B. „Genehmigung – SharePoint 2010“) hinzufügen.

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:

1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.

2. Wählen Sie unter **Websiteobjekte** **Workflows** aus.

3. Wählen Sie im Abschnitt **Neu** des Menübands **Workflows** die Option **Wiederverwendbarer Workflow** aus.

4. Geben Sie im Formular **"Wiederverwendbaren Workflow erstellen**" den Namen **_"Repair2010_*_" ein.* Klicken Sie für "_Plattformtyp**" auf **SharePoint 2010-Workflow**, und klicken Sie dann auf **"OK**".

   1. Wählen Sie im Abschnitt **„Speichern“** des Menübands **Workflow** die Option **Veröffentlichen** aus.

   2. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** die Option **Global veröffentlichen** aus. Wählen Sie im daraufhin angezeigten Bestätigungsdialogfeld **OK** aus.

   3. Suchen Sie in einem Webbrowser die Stammwebsite der Websitesammlung, und greifen Sie dann auf **website-Einstellungen** \> **Websitesammlungsfeatures** zu. Schalten Sie dann das **Workflowfeature** um:
      - Wenn das Feature *aktiviert* ist, klicken Sie auf **"Deaktivieren"** und dann auf **"Aktivieren"**.
      - Wenn das Feature *deaktiviert* ist, klicken Sie auf **"Aktivieren"**.

Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
