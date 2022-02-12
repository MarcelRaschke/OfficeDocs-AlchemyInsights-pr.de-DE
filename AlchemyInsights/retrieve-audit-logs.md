---
title: Abrufen der Überwachungsprotokolle
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: df89e0edd55bfc4ea840380efe91c0a50380e400
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62598250"
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
