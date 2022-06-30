---
title: Erstellen einer Freigaberichtlinie, um Ihren Benutzern die Freigabe ihrer Kalenderdaten für Personen außerhalb Ihrer Organisation zu erlauben
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 778d746a7adf6112a314e242b94eb5d69ebfa6e0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66423247"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>Erstellen einer Freigaberichtlinie, um Ihren Benutzern die Freigabe ihrer Kalenderdaten für Personen außerhalb Ihrer Organisation zu erlauben

1. Wechseln Sie vom Microsoft 365 Admin Center-Dashboard zu **Administrator** >  **Exchange** > **Organisation** > [**Freigabe**](https://admin.exchange.microsoft.com/#/sharing).
1. Wählen Sie in der Listenansicht unter **Einzelne Freigabe** **Neu** aus.
1. Geben Sie unter **Neue Freigaberichtlinie** einen Anzeigenamen für die Freigaberichtlinie im Feld **Richtlinienname** ein.
1. Wählen Sie **Hinzufügen** aus, um die Freigaberegeln für die Richtlinie zu definieren.
1. Wählen Sie im Dialogfeld **Freigaberegel** eine der folgenden Optionen aus, um die Domänen für die Freigabe anzugeben:
    - **Freigabe für alle Domänen**
    - **Freigabe für eine bestimmte Domäne**
1. Wenn Sie **Freigabe für eine bestimmte Domäne** auswählen, geben Sie die Domäne für die Freigabe ein. Wenn Sie mehr als eine Domäne für diese Freigaberichtlinie eingeben müssen, speichern Sie zunächst die Einstellungen für die erste Domäne. Bearbeiten Sie anschließend die Freigaberegeln, um weitere Domänen hinzuzufügen.
1. Zum Angeben der freizugebenden Informationen aktivieren Sie das Kontrollkästchen **Ihre Kalenderordner freigeben**. Wählen Sie anschließend eine der folgenden Optionen aus:
    - **Frei/Gebucht-Kalenderinformationen nur mit Zeit**
    - **Frei/Gebucht-Kalenderinformationen mit Zeit, Betreff und Ort**
    - **Alle Informationen zum Termin einschließlich Uhrzeit, Betreff, Ort und Titel**
1. Wählen Sie **Speichern** aus, um die Regeln für die Freigaberichtlinie festzulegen.
1. Wenn Sie diese Freigaberichtlinie als die neue Standardfreigaberichtlinie für alle Benutzer in Ihrer Organisation festlegen möchten, aktivieren Sie das Kontrollkästchen **Diese Richtlinie als meine Standardfreigaberichtlinie verwenden**.
1. Wählen Sie **Speichern** aus, um die Freigaberichtlinie zu erstellen.  

**Für vollständige Informationen zu diesem Thema lesen Sie:**

- [Erstellen einer Freigaberichtlinie in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [Anwenden von Freigaberichtlinien auf Postfächer in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [Ändern, Deaktivieren oder Entfernen einer Freigaberichtlinie in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)