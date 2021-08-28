---
title: Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331122"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen

Sie können die Überwachungsprotokollsuche im Microsoft 365 Compliance Center verwenden, um Posteingangsregelereignisse anzuzeigen (Erstellen, Ändern und Löschen von Posteingangsregeln).

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> "Lösungsüberwachung" zu **"Lösungsüberwachung".** \>  Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://compliance.microsoft.com/auditlogsearch> wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **"Überwachen".** Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://security.microsoft.com/auditlogsearch> wechseln.

2. Konfigurieren Sie auf der Registerkarte **"Suchen"** der **Überwachungsseite** die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich:** Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - **Aktivitäten:** Wählen Sie einen oder mehrere der folgenden Werte aus:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Aktualisieren von Posteingangsregeln von Outlook Client**

3. Wenn Sie fertig sind, klicken Sie auf **Suchen.** Die Aktivitäten werden auf der neuen **Überwachungssuchseite** angezeigt.

4. Wählen Sie eine Aktivität in den Ergebnissen aus, um das Detail-Flyout zu öffnen. Informationen zu den Posteingangsregeleinstellungen werden im **Parameterfeld** angezeigt.

Weitere Informationen finden Sie unter [Ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
