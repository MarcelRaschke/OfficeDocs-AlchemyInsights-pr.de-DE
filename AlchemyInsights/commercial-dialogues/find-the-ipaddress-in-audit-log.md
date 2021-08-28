---
title: Suchen der IP-Adresse im Überwachungsprotokoll
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902259"
---
# <a name="find-the-ip-address-in-audit-log"></a>Suchen der IP-Adresse im Überwachungsprotokoll

Die IP-Adresse, die einer von einem Benutzer oder Administrator ausgeführten Aktivität entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. So identifizieren Sie die IP-Adresse:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **"Lösungsüberwachung".** \>  Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://compliance.microsoft.com/auditlogsearch> wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **"Überwachen".** Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://security.microsoft.com/auditlogsearch> wechseln.

    > [!NOTE]
    > Wenn Sie einen Hinweis sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.

2. Überprüfen Sie auf der Seite **"Überwachung",** ob die Registerkarte **"Suchen"** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich:** Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - **Aktivitäten:** Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie aus der Liste aus. andernfalls wird der Standardwert **"Ergebnisse für alle Aktivitäten anzeigen"** zurückgegeben, der alle Aktivitäten zurückgibt. Beachten Sie, dass bestimmte Aktivitäten möglicherweise nicht für die Auswahl verfügbar sind. Diese Überwachungselemente werden jedoch zurückgegeben, wenn **"Ergebnisse für alle Aktivitäten anzeigen"** ausgewählt ist.
   - **Benutzer:** Akzeptieren Sie den leeren Standardwert, um Ergebnisse für alle Benutzer zurückzugeben, oder geben Sie einen oder mehrere Benutzer ein.

3. Wenn Sie fertig sind, klicken Sie auf **Suchen.** Die Aktivitäten werden auf der neuen **Überwachungssuchseite** angezeigt.

4. Klicken Sie in den Ergebnissen auf **"Ergebnisse filtern",** und geben **Sie "Set-Mailbox"** im Aktivitätsfilterfeld ein.

5. Wählen Sie einen Überwachungsdatensatz in den Ergebnissen aus, um das **Flyout "Details"** zu öffnen.

Weitere Informationen finden Sie unter [Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
