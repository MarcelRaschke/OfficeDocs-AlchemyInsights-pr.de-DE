---
title: Zulassen oder Deaktivieren von IP-Video in Teams
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: e2048b12c066412a99bf8405230c96edfb259943
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63198356"
---
# <a name="teams-allow-or-disable-ip-video"></a>Zulassen oder Deaktivieren von IP-Video in Teams

**Ändern oder Erstellen einer Besprechungsrichtlinie**

Um eine Besprechungsrichtlinie zu ändern oder zu erstellen, wechseln Sie zu **Microsoft Teams Admin Center > Besprechungen > Besprechungsrichtlinien**. Wählen Sie in der Liste eine Richtlinie aus, oder klicken Sie auf **Hinzufügen**. Wenn Sie eine neue Richtlinie erstellen, fügen Sie einen Namen und eine Beschreibung hinzu. Der Name darf keine Sonderzeichen enthalten und nicht mehr als 64 Zeichen lang sein. Wählen Sie die gewünschten Einstellungen aus, und klicken Sie dann auf **Speichern**.

Nehmen wir beispielsweise an, Sie haben viele Benutzer, und Sie möchten die Bandbreite begrenzen, die für deren Besprechung erforderlich ist. Sie erstellen dann eine neue benutzerdefinierte Richtlinie namens „begrenzte Bandbreite“ und deaktivieren die folgenden Einstellungen:

Unter **Audio & Video**:

- Deaktivieren Sie Cloud-Aufzeichnung zulassen.
- Deaktivieren Sie IP-Video zulassen.

Weisen Sie dann die Richtlinie den Nutzern zu.

**Nutzern eine Besprechungsrichtlinie zuweisen**

1. Wechseln Sie in der linken Navigation des Microsoft Teams Admin Centers zu **Nutzer**, und klicken Sie dann den gewünschten Nutzer an.
2. Wählen Sie den Nutzer aus, indem Sie links neben den Nutzernamen klicken, und klicken Sie dann auf **Einstellungen bearbeiten**.
3. Wählen Sie unter **Besprechungsrichtlinie** die Richtlinie aus, die Sie zuweisen möchten, und klicken Sie dann auf **Übernehmen**.

Weitere Informationen finden Sie unter [Besprechungsrichtlinien in Teams verwalten](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
