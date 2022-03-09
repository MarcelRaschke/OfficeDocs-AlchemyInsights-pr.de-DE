---
title: So wird eine Vertraulichkeitsbezeichnung veröffentlicht
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "11015"
- "9000181"
ms.openlocfilehash: 3376cc32d93d1e9e09030eab5354fd5dee22f1ab
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63294391"
---
# <a name="how-to-publish-a-sensitivity-label"></a>So wird eine Vertraulichkeitsbezeichnung veröffentlicht

1. Wechseln Sie zum Microsoft 365 Compliance Center > **Information Protection** > **Bezeichnungsrichtlinien**.

1. Wählen Sie **+ Bezeichnung veröffentlichen** aus, um den Assistenten für neue Vertraulichkeitsbezeichnungen zu starten.

1. Wählen Sie **Zu veröffentlichende Vertraulichkeitsbezeichnungen auswählen** aus. Wählen Sie die Bezeichnungen, die Sie in Apps und Diensten zur Verfügung stellen möchten, und dann **Hinzufügen** aus.

    **Wichtig**: Wenn Sie eine Unterbezeichnung auswählen, stellen Sie sicher, dass Sie auch deren übergeordnete Bezeichnung auswählen.

1. Überprüfen Sie die ausgewählten Bezeichnungen. Um Änderungen vorzunehmen, wählen Sie **Bearbeiten** aus; andernfalls wählen Sie **Weiter** aus.

1. Folgen Sie den Eingabeaufforderungen, um die Richtlinieneinstellungen zu konfigurieren.

1. Wiederholen Sie diese Schritte, wenn Sie für verschiedene Benutzer oder Standorte unterschiedliche Richtlinieneinstellungen benötigen. Sie möchten z. B. zusätzliche Bezeichnungen für eine Gruppe von Benutzern oder eine andere Standardbezeichnung für eine Untergruppe von Benutzern festlegen.

1. Wenn Sie mehrere Bezeichnungsrichtlinie erstellen, die zu einem Konflikt für einen Benutzer oder Standort führen könnten, überprüfen Sie die Reihenfolge der Richtlinien und verschieben Sie einzelne Richtlinien gegebenenfalls nach oben oder unten. Um die Reihenfolge einer Bezeichnungsrichtlinie zu ändern, wählen Sie die drei Punkte (weitere Aktionen) und wählen Sie dann **Nach oben verschieben** oder **Nach unten verschieben** aus.

Nach Abschluss des Assistenten wird die Bezeichnungsrichtlinie automatisch veröffentlicht.

Weitere Informationen finden Sie unter [Erstellen und Konfigurieren von Vertraulichkeitsbezeichnungen und deren Richtlinien](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels).