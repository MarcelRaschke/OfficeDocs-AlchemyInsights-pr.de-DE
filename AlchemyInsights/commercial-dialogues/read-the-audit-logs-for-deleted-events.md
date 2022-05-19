---
title: Lesen der Überwachungsprotokolle für gelöschte Ereignisse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d926de720f120443685ba900c10fdfad4f0a4f03
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65592544"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Lesen der Überwachungsprotokolle für gelöschte Ereignisse

Gehen Sie dazu wie folgt vor:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie in der Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com>zu **"Lösungsüberwachung"**\>. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

    **Hinweis**: Wenn ein Hinweis angezeigt wird, dass Sie das Feature aktivieren müssen, fahren Sie fort, und aktivieren Sie es jetzt. Wenn das Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus vorherigen Datumsangaben abrufen.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " auf der Seite " **Überwachung** " die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Geben Sie **Exchange Postfachaktivitäten** ein, und wählen Sie dann die folgenden Werte aus:
     - **Nachrichten aus Ordner „Gelöschte Elemente“ gelöscht**
     - **Nachrichten in Ordner "Gelöschte Elemente" verschoben**

       Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, **um den** Aktivitätenbereich zu minimieren.

   - **Benutzer**: Übernehmen Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, bzw. geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie in den Ergebnissen eine Aktivität aus, um das Detail-Flyout zu öffnen. Zusätzliche Informationen zum gelöschten Element, z. B. die Betreffzeile und die Position des Elements, als es gelöscht wurde, werden im Feld **"Betroffene Elemente** " angezeigt.

   **Hinweis**: Sie können gelöschte Elemente nicht mithilfe des Überwachungsprotokollfeatures wiederherstellen. Informationen zum Wiederherstellen gelöschter Elemente finden [Sie unter Wiederherstellen gelöschter E-Mail-Nachrichten in Outlook im Web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Weitere Informationen finden [Sie unter Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
