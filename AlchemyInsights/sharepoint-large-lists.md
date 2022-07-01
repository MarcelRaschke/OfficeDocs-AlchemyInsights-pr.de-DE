---
title: Große SharePoint-Listen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "530001"
- "407"
ms.date: 04/21/2020
ms.openlocfilehash: c9d01dd5cb0907974edbf38806720bc29b278e17
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66590179"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeiten mit umfangreichen Listen und Bibliotheken in SharePoint

SharePoint-Listen und -Bibliotheken können bis zu 30 Millionen Elemente enthalten, aber wenn sie mehr als 5.000 Elemente enthalten, wird möglicherweise ein Schwellenwert für die Listenansicht angezeigt, wenn Sie versuchen, mit ihnen zu arbeiten. Dieser Schwellenwert dient dazu, die Leistung des Diensts aufrechtzuerhalten. Er kann nicht geändert werden. So vermeiden Sie das Erreichen dieses Schwellenwerts:

**Modernes verwenden**

Ansichten, in denen viele Elemente angezeigt werden, funktionieren in der modernen Benutzeroberfläche am besten. [Verwenden Sie die moderne Oberfläche](https://support.microsoft.com/office/switch-the-default-experience-for-lists-and-libraries-from-new-or-classic-66dac24b-4177-4775-bf50-3d267318caa9) , um Fehler zu vermeiden, die in der klassischen Benutzeroberfläche auftreten können.

**Hinzufügen von Indizes**

Wenn Sie nach einer Spalte filtern oder sortieren, die keinen Index hat, wird möglicherweise eine Fehlermeldung angezeigt. [Fügen Sie einen Index](https://support.microsoft.com/office/add-an-index-to-a-list-or-library-column-f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuell aus den **Listeneinstellungen** im Menü "Einstellungen" und dann " **Indizierte Spalten**" hinzu.

**Bearbeiten der Listenansicht**

Wenn beim Arbeiten mit einer großen Liste ein Fehler auftritt, [bearbeiten Sie die Listenansicht](https://support.microsoft.com/office/edit-a-view-of-a-list-15916903-e79a-423f-b4e2-02d37e1ff372).

Mit den folgenden vier Änderungen werden Fehler beim Schwellenwert für die Listenansicht entfernt. Nehmen Sie alle vier Änderungen vor, um alle Fehler zu entfernen. Wenn weiterhin Fehler auftreten, aktivieren Sie " [Große Listen und Bibliotheken verwalten](https://support.microsoft.com/office/manage-large-lists-and-libraries-b8588dae-9387-48c2-9248-c24122f07c59)".

1. Wählen Sie **"Keine"** aus der **ersten Sortierung nach der Spalte** und **dann nach der Spalte aus**.
2. Wählen Sie **"Keine"** aus der **ersten Gruppe nach der Spalte** und **dann nach der Spalte** aus.
3. Wählen Sie **"Keine"** für alle Spalten im Abschnitt **"Summen** " aus.
4. Heben Sie die Auswahl aller Spalten bis auf eine Spalte auf, die im Abschnitt **"Spalten** " angezeigt werden soll.

