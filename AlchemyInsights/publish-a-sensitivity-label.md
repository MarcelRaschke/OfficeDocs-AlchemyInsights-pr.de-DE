---
title: So wird eine Vertraulichkeitsbezeichnung veröffentlicht
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000181"
- "11015"
ms.date: 04/21/2021
ms.openlocfilehash: da3894ab316397ac57d4e54cfe379e476c5e6fa6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66265492"
---
# <a name="how-to-publish-a-sensitivity-label"></a>So wird eine Vertraulichkeitsbezeichnung veröffentlicht

1. Wechseln Sie zu Microsoft Purview-Complianceportal > **Information Protection** > **Bezeichnungsrichtlinien**.

1. Wählen Sie **+ Bezeichnung veröffentlichen** aus, um den Assistenten für neue Vertraulichkeitsbezeichnungen zu starten.

1. Wählen Sie **Zu veröffentlichende Vertraulichkeitsbezeichnungen auswählen** aus. Wählen Sie die Bezeichnungen, die Sie in Apps und Diensten zur Verfügung stellen möchten, und dann **Hinzufügen** aus.

    **Wichtig**: Wenn Sie eine Unterbezeichnung auswählen, stellen Sie sicher, dass Sie auch deren übergeordnete Bezeichnung auswählen.

1. Überprüfen Sie die ausgewählten Bezeichnungen. Um Änderungen vorzunehmen, wählen Sie **Bearbeiten** aus; andernfalls wählen Sie **Weiter** aus.

1. Folgen Sie den Eingabeaufforderungen, um die Richtlinieneinstellungen zu konfigurieren.

1. Wiederholen Sie diese Schritte, wenn Sie für verschiedene Benutzer oder Standorte unterschiedliche Richtlinieneinstellungen benötigen. Sie möchten z. B. zusätzliche Bezeichnungen für eine Gruppe von Benutzern oder eine andere Standardbezeichnung für eine Untergruppe von Benutzern festlegen.

1. Wenn Sie mehrere Bezeichnungsrichtlinie erstellen, die zu einem Konflikt für einen Benutzer oder Standort führen könnten, überprüfen Sie die Reihenfolge der Richtlinien und verschieben Sie einzelne Richtlinien gegebenenfalls nach oben oder unten. Um die Reihenfolge einer Bezeichnungsrichtlinie zu ändern, wählen Sie die drei Punkte (weitere Aktionen) und wählen Sie dann **Nach oben verschieben** oder **Nach unten verschieben** aus.

Nach Abschluss des Assistenten wird die Bezeichnungsrichtlinie automatisch veröffentlicht.

Weitere Informationen finden Sie unter [Erstellen und Konfigurieren von Vertraulichkeitsbezeichnungen und deren Richtlinien](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels).