---
title: Abrufen der Überwachungsprotokolle
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3100005"
- "10964"
ms.date: 04/16/2021
ms.openlocfilehash: 47d12d9dec297c1b468374475060e0d9ee288a4a
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66263962"
---
# <a name="retrieve-the-audit-logs"></a>Abrufen der Überwachungsprotokolle

Wenn Sie das Überwachungsprotokoll zum ersten Mal öffnen, ist es leer. Sie müssen eine Suche durchführen, um zu sehen, was da ist. So führen Sie eine allgemeine Suche nach allen Aktivitäten durch:

1. Führen Sie einen der folgenden Schritte aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Vergewissern Sie sich, dass **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist.
   - **Benutzer**: Übernehmen Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, bzw. geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf **Ergebnisse filtern**, und geben Sie **Set-Mailbox** in das Aktivitätsfilterfeld ein.

5. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im angezeigten Detailflyout können Sie weitere Informationen anzeigen, z. B. den Client, den Benutzer, der eine Aktion ausgeführt hat, und so weiter.
