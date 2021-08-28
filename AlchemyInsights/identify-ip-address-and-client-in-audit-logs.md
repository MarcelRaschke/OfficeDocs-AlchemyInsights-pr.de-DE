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
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313018"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen

Die IP-Adresse, die einer Aktivität eines Microsoft 365 Benutzers oder Administrators entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. Hier sind die Schritte zum Identifizieren dieser Informationen

1. Melden Sie sich beim [Microsoft 365 Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur Suchseite des  >  **Überwachungsprotokolls** für die Suche.

   Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie aus der Liste **"Aktivitäten"** aus. Wenn nicht, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).

   **Hinweis:** Bestimmte Aktivitäten sind möglicherweise nicht im Menü **"Aktivitäten"** verfügbar. Diese Überwachungselemente werden jedoch zurückgegeben, wenn **"Ergebnisse für alle Aktivitäten anzeigen"** ausgewählt ist (Standardeinstellung).

3. Geben Sie den Benutzernamen im Feld **"Benutzer"** an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **"Suchen".**

In den Ergebnissen sehen Sie die IP-Adresse für diese Aktivität im Ergebnisbereich. Wählen Sie den Überwachungsdatensatz  aus, um detaillierte Informationen im Detail-Flyout anzuzeigen (z. B. Client, Benutzer, der eine Aktion ausgeführt hat usw.).

Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet wird.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
