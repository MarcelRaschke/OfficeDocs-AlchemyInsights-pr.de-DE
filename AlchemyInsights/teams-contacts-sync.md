---
title: Teams-Kontaktsynchronisierung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: eb157236df20506eebb8680af7cf3afe6767e061
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66383169"
---
# <a name="teams-contacts-sync"></a>Teams-Kontaktsynchronisierung

Teams verwendet Kontakte im Active Directory Ihrer Organisation sowie Kontakte, die dem Outlook-Standardordner des Benutzers hinzugefügt wurden. Wenn Kontakte nicht in Microsoft Teams angezeigt werden, versuchen Sie Folgendes:

**Hinweis:** Wenn die Informationen für einen oder mehrere Kontakte kürzlich aktualisiert wurden, kann es bis zu 48 Stunden dauern, bis die Kontakte synchronisiert sind.

1. Melden Sie sich bei Teams ab und starten Sie es neu. Überprüfen Sie, ob Ihre Kontakte angezeigt werden.
1. Löschen Sie den Teams-Cache:
    1. Browsen Sie zu **%appdata%\Microsoft\Teams**.
    1. Löschen Sie den Inhalt des Ordners.
    1. Starten Sie den Computer neu und versuchen Sie, Teams zu starten.
1. Wenn sich der Kontakt in Outlook befindet, stellen Sie sicher, dass er der Kontaktliste hinzugefügt wird. Wählen Sie in Outlook in der Adressleiste **Datei** aus, und wählen Sie dann **Zu Kontakten hinzufügen** aus.
1. Stellen Sie sicher, dass das Exchange-Postfach online gehostet ist (nicht lokal). Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
1. Stellen Sie sicher, dass die Telefonnummer des Kontaktes zu den Kontaktinformationen hinzugefügt ist.
1. Suchen Sie in der Suchleiste nach der E-Mail des Kontakts. Kontakte, die Sie mit der Kontaktliste synchronisieren können.
