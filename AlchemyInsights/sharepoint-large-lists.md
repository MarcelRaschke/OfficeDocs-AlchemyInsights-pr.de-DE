---
title: SharePoint große Listen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 09dff8362631ee8fabc4a6661b918e3e1aaeabcb
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61957021"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeiten mit großen Listen und Bibliotheken in SharePoint

SharePoint Listen und Bibliotheken können bis zu 30 Millionen Elemente enthalten, aber wenn sie mehr als 5.000 Elemente enthalten, wird beim Versuch, mit ihnen zu arbeiten, möglicherweise ein Schwellenwert für die Listenansicht angezeigt. Dieser Schwellenwert dient dazu, die Leistung des Diensts aufrechtzuerhalten. Er kann nicht geändert werden. So vermeiden Sie das Erreichen dieses Schwellenwerts:

**Modern verwenden**

Ansichten mit vielen Elementen funktionieren am besten in der modernen Benutzeroberfläche. [Verwenden Sie die moderne Benutzeroberfläche,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) um Fehler zu vermeiden, die möglicherweise in der klassischen Benutzeroberfläche angezeigt werden.

**Hinzufügen von Indizes**

Wenn Sie nach einer Spalte filtern oder sortieren, die keinen Index aufweist, wird möglicherweise eine Fehlermeldung angezeigt. [Fügen Sie einen Index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuell aus listen **Einstellungen** im Einstellungsmenü und dann **indizierten Spalten** hinzu.

**Bearbeiten der Listenansicht**

Wenn beim Arbeiten mit einer großen Liste ein Fehler auftritt, [bearbeiten Sie die Listenansicht.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)

Die folgenden vier Änderungen entfernen Schwellenwertfehler bei der Listenansicht. Nehmen Sie alle vier Änderungen vor, um alle Fehler zu entfernen. Wenn weiterhin Fehler auftreten, überprüfen Sie ["Verwalten großer Listen und Bibliotheken".](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Wählen Sie **Keine** aus **der ersten Sortierung nach der Spalte** und dann nach der **Spalte** aus.
2. Wählen Sie **keine** aus der **ersten Gruppe nach der Spalte** und dann nach der Spalte **gruppieren.**
3. Wählen Sie im Abschnitt **Summen** für alle Spalten Keine aus. 
4. Deaktivieren Sie die Auswahl aller Spalten bis auf eine Spalte für die Anzeige im Abschnitt **"Spalten".**

