---
title: Suchen von Ereignissen, die für Posteingangsregeln ausgeführt wurden
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
ms.openlocfilehash: b6e2471b4ab2e387350817c5a4773c711c1ad9c0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66414152"
---
# <a name="find-events-performed-on-inbox-rules"></a>Suchen von Ereignissen, die für Posteingangsregeln ausgeführt wurden

Wenn Posteingangsregeln erstellt, geändert oder gelöscht werden, werden die Ereignisse im Überwachungsprotokoll aufgezeichnet. Hier erfahren Sie, wie Sie sie überprüfen:

1. Führen Sie eine der folgenden Aktionen aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

    **Hinweis**: Wenn eine Benachrichtigung angezeigt wird, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus vorherigen Datumsangaben abrufen.
1. Wählen Sie das Feld "Aktivitäten" aus, suchen Sie Exchange-Postfachaktivitäten, und wählen Sie dann New-InboxRule Posteingangsregel aus Outlook Web App erstellen aus. Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den Aktivitätenbereich zu minimieren.
1. Geben Sie den Datumsbereich an, und wählen Sie dann im Feld "Benutzer" den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten. Sie können mehrere Benutzer gleichzeitig auswählen.
1. Wählen Sie Suchen aus. Die Aktivitäten werden unter Ergebnisse angezeigt.
1. Um Details anzuzeigen, wählen Sie eine Aktivität aus, und wählen Sie dann "Weitere Informationen" aus. Im Abschnitt "Parameter" werden der Name der Regel, die festgelegten Bedingungen und die Aktionen angezeigt, die von der Regel ausgeführt werden.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " auf der Seite " **Überwachung** " die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Auswählen **von "Neuer PosteingangRule Posteingangsregel erstellen" aus Outlook Web App**

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie in den Ergebnissen eine Aktivität aus, um das Detail-Flyout zu öffnen. Im Abschnitt **"Parameter** " werden der Name der Regel, die festgelegten Bedingungen und die Aktionen angezeigt, die von der Regel ausgeführt werden.

Weitere Informationen finden [Sie unter Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
