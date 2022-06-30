---
title: Identifizieren von IP-Adresse und Client in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100005"
- "1367"
ms.date: 04/21/2020
ms.openlocfilehash: f2b2c2bc2ccef36e34a6f76759a504171f559db0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66376203"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifizieren von IP-Adresse und Client in Überwachungsprotokollen

Die IP-Adresse, die einer Aktivität eines Microsoft 365-Benutzers oder -Administrators entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. Hier sind die Schritte zum Identifizieren solcher Informationen.

1. Führen Sie einen der folgenden Schritte aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " auf der Seite " **Überwachung** " die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **"Start** " und " **Ende** " aus.
   - **Aktivitäten**: Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie aus der Liste aus. Andernfalls werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).

     **Hinweis**: Bestimmte Aktivitäten sind möglicherweise nicht im Menü **"Aktivitäten** " verfügbar; Diese Überwachungselemente werden jedoch zurückgegeben, wenn " **Ergebnisse für alle Aktivitäten anzeigen"** ausgewählt ist (Standardeinstellung).

   - **Benutzer**: Geben Sie den Benutzernamen an.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. In den Ergebnissen wird die IP-Adresse für diese Aktivität angezeigt. Wenn Sie einen Überwachungsdatensatz auswählen, wird das Detail-Flyout angezeigt, in dem Sie zusätzliche Informationen sehen können (z. B. Client, Benutzer, der eine Aktion ausgeführt hat usw.).

Weitere Informationen finden Sie unter [Ermitteln der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet wird](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
