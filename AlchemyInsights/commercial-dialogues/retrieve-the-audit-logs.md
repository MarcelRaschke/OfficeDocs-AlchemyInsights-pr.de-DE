---
title: Abrufen der Überwachungsprotokolle
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: dad0f74201eecc876f30d53bb1dc4e47a1cd5fca
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62671963"
---
# <a name="retrieve-the-audit-logs"></a>Abrufen der Überwachungsprotokolle

Wenn Sie das Überwachungsprotokoll zum ersten Mal öffnen, ist es leer. Sie müssen eine Suche durchführen, um zu sehen, was da ist. So führen Sie eine allgemeine Suche nach allen Aktivitäten durch:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " der **Überwachungsseite** die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Vergewissern Sie sich, dass **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist.
   - **Benutzer**: Übernehmen Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, bzw. geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie eine Aktivität in den Ergebnissen aus, um das Detail-Flyout zu öffnen. Es werden weitere Informationen angezeigt, z. B. Client, Benutzer, der eine Aktion ausgeführt hat usw.

Weitere Informationen finden Sie unter [Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
