---
title: Abrufen der Überwachungsprotokolle
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: d94cd0791d55b6355cbb56549bf8861156d0ebc8
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799830"
---
# <a name="retrieve-the-audit-logs"></a>Abrufen der Überwachungsprotokolle

Wenn Sie das Überwachungsprotokoll zum ersten Mal öffnen, ist es leer. Sie müssen eine Suche durchführen, um zu sehen, was da ist. So führen Sie eine allgemeine Suche nach allen Aktivitäten durch:

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Vergewissern Sie sich, dass **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist.
   - **Benutzer**: Übernehmen Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, bzw. geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf **Ergebnisse filtern**, und geben Sie **Set-Mailbox** in das Aktivitätsfilterfeld ein.

5. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im angezeigten Detailflyout können Sie weitere Informationen anzeigen, z. B. den Client, den Benutzer, der eine Aktion ausgeführt hat, und so weiter.
