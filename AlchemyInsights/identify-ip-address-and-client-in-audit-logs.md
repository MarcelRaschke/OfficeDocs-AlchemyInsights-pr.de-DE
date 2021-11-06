---
title: Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bea29b9d0f3b0f612f9a6e5ca65550cca1d717b6
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799218"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen

Die IP-Adresse, die einer Aktivität eines Microsoft 365 Benutzers oder Administrators entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. Hier sind die Schritte zum Identifizieren dieser Informationen.

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Konfigurieren Sie auf der Registerkarte **"Suchen"** der **Überwachungsseite** die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - **Aktivitäten:** Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie aus der Liste aus. Wenn nicht, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).

     **Hinweis:** Bestimmte Aktivitäten sind möglicherweise nicht im Menü **"Aktivitäten"** verfügbar. Diese Überwachungselemente werden jedoch zurückgegeben, wenn **"Ergebnisse für alle Aktivitäten anzeigen"** ausgewählt ist (Standardeinstellung).

   - **Benutzer:** Geben Sie den Benutzernamen an.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. In den Ergebnissen sehen Sie die IP-Adresse für diese Aktivität. Wenn Sie einen Überwachungsdatensatz auswählen, wird das Detail-Flyout angezeigt, in dem Sie zusätzliche Informationen sehen können (z. B. Client, Benutzer, der eine Aktion ausgeführt hat usw.).

Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet wird.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
