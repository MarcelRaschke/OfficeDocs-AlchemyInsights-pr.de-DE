---
title: Teams-Kontaktsynchronisierung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: 94d260e58e0a6e8d1f82dca262becbf875444499
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62750771"
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
