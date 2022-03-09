---
title: Genehmigungsworkflow 2010 kann nicht hinzugefügt werden
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 12cd797f1108afb355baa50fd0f101686d219f6c
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63289925"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Genehmigungsworkflow 2010 kann nicht hinzugefügt werden

In einer Microsoft SharePoint-Websitesammlung können Sie zu einer Liste oder Bibliothek keinen global wiederverwendbaren Workflow (z. B. „Genehmigung – SharePoint 2010“) hinzufügen.
  
Gehen Sie folgendermaßen vor, um dieses Problem zu beheben: 
  
1. Öffnen Sie die Stammwebsite der Websitesammlung in SharePoint Designer 2013.
  
2. Wählen Sie unter **Websiteobjekte** **Workflows** aus. 
  
3. Wählen Sie im Abschnitt **Neu** des Menübands **Workflows** die Option **Wiederverwendbarer Workflow** aus. 
  
4. Geben Sie im Formular " **Wiederverwendbarer Workflow erstellen** " den Namen ** *Repair2010* ** ein. Klicken Sie für den **Plattformtyp** auf **SharePoint 2010-Workflow**, und klicken Sie dann auf **OK**. 
  
1. Wählen Sie im Abschnitt **„Speichern“** des Menübands **Workflow** die Option **Veröffentlichen** aus. 
  
2. Wählen Sie im Abschnitt **Verwalten** des Menübands **Workflow** die Option **Global veröffentlichen** aus. Wählen Sie im daraufhin angezeigten Bestätigungsdialogfeld **OK** aus. 
  
3. Suchen Sie in einem Webbrowser nach der Stammwebsite der Websitesammlung, und greifen Sie dann auf **Website Einstellungen** \> **Websitesammlungsfeatures** zu. Umschalten des **Workflows-Features** : 
  
· Wenn das Feature  *aktiviert*  ist, klicken Sie auf **"Deaktivieren** " und dann auf " **Aktivieren**". 
  
· Wenn das Feature  *deaktiviert*  ist, klicken Sie auf **"Aktivieren**". 
  
Weitere Informationen finden Sie im folgenden [Artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

