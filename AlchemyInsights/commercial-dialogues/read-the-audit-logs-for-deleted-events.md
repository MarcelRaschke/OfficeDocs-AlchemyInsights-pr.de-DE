---
title: Lesen der Überwachungsprotokolle für gelöschte Ereignisse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100005"
- "7327"
ms.date: 02/26/2021
ms.openlocfilehash: af142e03f8495aba6c6b49eabcb2fe22a5e58065
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66368787"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Lesen der Überwachungsprotokolle für gelöschte Ereignisse

Gehen Sie dazu wie folgt vor:

1. Führen Sie eine der folgenden Aktionen aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

    **Hinweis**: Wenn ein Hinweis angezeigt wird, dass Sie das Feature aktivieren müssen, fahren Sie fort, und aktivieren Sie es jetzt. Wenn das Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus vorherigen Datumsangaben abrufen.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " auf der Seite " **Überwachung** " die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Geben Sie **Exchange-Postfachaktivitäten ein** , und wählen Sie dann die folgenden Werte aus:
     - **Nachrichten aus Ordner „Gelöschte Elemente“ gelöscht**
     - **Nachrichten in Ordner "Gelöschte Elemente" verschoben**

       Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, **um den** Aktivitätenbereich zu minimieren.

   - **Benutzer**: Übernehmen Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, bzw. geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie in den Ergebnissen eine Aktivität aus, um das Detail-Flyout zu öffnen. Zusätzliche Informationen zum gelöschten Element, z. B. die Betreffzeile und die Position des Elements, als es gelöscht wurde, werden im Feld **"Betroffene Elemente** " angezeigt.

   **Hinweis**: Sie können gelöschte Elemente nicht mithilfe des Überwachungsprotokollfeatures wiederherstellen. Informationen zum Wiederherstellen gelöschter Elemente finden [Sie unter Wiederherstellen gelöschter E-Mail-Nachrichten in Outlook im Web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Weitere Informationen finden [Sie unter Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
