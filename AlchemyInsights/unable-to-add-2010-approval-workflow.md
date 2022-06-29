---
title: Genehmigungsworkflow 2010 kann nicht hinzugefügt werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.date: 04/21/2020
ms.openlocfilehash: 5e7ec7448e6e67ee6f97644f0dd65f71cca7fb05
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66279118"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Genehmigungsworkflow 2010 kann nicht hinzugefügt werden

In einer Microsoft SharePoint-Websitesammlung können Sie zu einer Liste oder Bibliothek keinen global wiederverwendbaren Workflow (z. B. „Genehmigung – SharePoint 2010“) hinzufügen.

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:

1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.

2. Wählen Sie unter **Websiteobjekte** **Workflows** aus.

3. Wählen Sie im Abschnitt **Neu** des Menübands **Workflows** die Option **Wiederverwendbarer Workflow** aus.

4. Geben Sie im Formular **"Wiederverwendbaren Workflow erstellen** " den Namen **_"Repair2010_*_" ein. Klicken Sie für "_* Plattformtyp**" auf **"SharePoint 2010-Workflow**" und dann auf **"OK**".

   1. Wählen Sie im Abschnitt **„Speichern“** des Menübands **Workflow** die Option **Veröffentlichen** aus.

   2. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** die Option **Global veröffentlichen** aus. Wählen Sie im daraufhin angezeigten Bestätigungsdialogfeld **OK** aus.

   3. Suchen Sie in einem Webbrowser die Stammwebsite der Websitesammlung, und greifen Sie dann auf **Websiteeinstellungen-Websitesammlungsfeatures** \> zu. Umschalten des **Workflows-Features** :
      - Wenn das Feature *aktiviert* ist, klicken Sie auf **"Deaktivieren"** und dann auf **"Aktivieren"**.
      - Wenn das Feature *deaktiviert* ist, klicken Sie auf **"Aktivieren"**.

Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
