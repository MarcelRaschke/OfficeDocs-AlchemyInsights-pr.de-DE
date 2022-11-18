---
title: Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen
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
- "1368"
ms.date: 04/21/2020
ms.openlocfilehash: 55cd5d247941ccf0f6d74a054e96a00861125d31
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66376144"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen

Sie können die Überwachungsprotokollsuche im Microsoft Purview-Complianceportal verwenden, um Posteingangsregelereignisse anzuzeigen (Erstellen, Ändern und Löschen von Posteingangsregeln).

1. Führen Sie einen der folgenden Schritte aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " auf der Seite " **Überwachung** " die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Wählen Sie einen oder mehrere der folgenden Werte aus:
     - **New-InboxRule Erstellen einer Posteingangsregel aus Outlook Web App**
     - **Set-InboxRule Regel von Outlook Web App ändern**.
     - **Aktualisieren von Posteingangsregeln vom Outlook-Client**

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie in den Ergebnissen eine Aktivität aus, um das Detail-Flyout zu öffnen. Informationen zu den Einstellungen der Posteingangsregel werden im Feld **"Parameter** " angezeigt.

Weitere Informationen finden Sie unter [Ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
