---
title: Untersuchen aller Benutzeraktivitäten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 2506eb7a122bff3a203d0ff45f17985c21ce6668
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65593084"
---
# <a name="investigate-all-the-users-activities"></a>Untersuchen aller Benutzeraktivitäten

Gehen Sie dazu wie folgt vor:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie in der Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com>zu **"Lösungsüberwachung"**\>. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

    **Hinweis**: Wenn ein Hinweis angezeigt wird, dass Sie das Feature aktivieren müssen, fahren Sie fort, und aktivieren Sie es jetzt. Wenn das Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus vorherigen Datumsangaben abrufen.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " auf der Seite " **Überwachung** " die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie aus der Liste aus. andernfalls gibt der Standardwert **"Ergebnisse für alle Aktivitäten anzeigen"** alle Aktivitäten zurück.
   - **Benutzer**: Übernehmen Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, bzw. geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt. Der **Name der IP-Adresse**, des **Benutzers** und der **Aktivität** wird angezeigt.

4. Um die Ergebnisse herunterzuladen, wählen Sie "**Alle Ergebnisse herunterladen"** **aus**\>.

5. Wählen Sie in den Ergebnissen eine Aktivität aus, um das Detail-Flyout zu öffnen.

Weitere Informationen finden [Sie unter Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
