---
title: Erstellen einer Freigaberichtlinie, um Ihren Benutzern die Freigabe ihrer Kalenderdaten für Personen außerhalb Ihrer Organisation zu erlauben
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
- "3800014"
- "898"
ms.openlocfilehash: 7a47eae7f55d3591fc06c8bd69ebd88e008b65f7
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63131825"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>Erstellen einer Freigaberichtlinie, um Ihren Benutzern die Freigabe ihrer Kalenderdaten für Personen außerhalb Ihrer Organisation zu erlauben

1. Wechseln Sie vom Microsoft 365 Admin Center-Dashboards zu **Admin** > **Exchange**.
2. Wechseln Sie zu **Organisation** > **Freigabe**.
3. Klicken Sie in der Listenansicht unter **Einzelne Freigabe** auf **Neu**.
4. Geben Sie unter **Neue Freigaberichtlinie** einen Anzeigenamen für die Freigaberichtlinie im Feld **Richtlinienname** ein.
5. Klicken Sie auf **Hinzufügen**, um die Freigaberegeln für die Richtlinie zu definieren.
6. Wählen Sie im Dialogfeld **Freigaberegel** eine der folgenden Optionen aus, um die Domänen für die Freigabe anzugeben:
    - **Freigabe für alle Domänen**
    - **Freigabe für eine bestimmte Domäne**
8. Wenn Sie **Freigabe für eine bestimmte Domäne** auswählen, geben Sie die Domäne für die Freigabe ein. Wenn Sie mehr als eine Domäne für diese Freigaberichtlinie eingeben müssen, speichern Sie zunächst die Einstellungen für die erste Domäne. Bearbeiten Sie anschließend die Freigaberegeln, um weitere Domänen hinzuzufügen.
9. Zum Angeben der freizugebenden Informationen aktivieren Sie das Kontrollkästchen **Ihre Kalenderordner freigeben**. Wählen Sie anschließend eine der folgenden Optionen aus:
    - **Frei/Gebucht-Kalenderinformationen nur mit Zeit**
    - **Frei/Gebucht-Kalenderinformationen mit Zeit, Betreff und Ort**
    - **Alle Informationen zum Termin einschließlich Uhrzeit, Betreff, Ort und Titel**
11. Klicken Sie auf **Speichern**, um die Regeln für die Freigaberichtlinie festzulegen.
12. Wenn Sie diese Freigaberichtlinie als die neue Standardfreigaberichtlinie für alle Benutzer in Ihrer Organisation festlegen möchten, aktivieren Sie das Kontrollkästchen **Diese Richtlinie als meine Standardfreigaberichtlinie verwenden**.
13. Klicken Sie auf **Speichern**, um die Freigaberichtlinie zu erstellen.  

**Für vollständige Informationen zu diesem Thema lesen Sie:**

- [Erstellen einer Freigaberichtlinie in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [Anwenden von Freigaberichtlinien auf Postfächer in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [Ändern, Deaktivieren oder Entfernen einer Freigaberichtlinie in Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)