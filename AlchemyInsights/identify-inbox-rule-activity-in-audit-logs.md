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
ms.localizationpriority: medium
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 15682a213bad9fbac094efb736cc51964e47a9b3
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63275561"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifizieren von Posteingangsregelaktivitäten in Überwachungsprotokollen

Sie können die Überwachungsprotokollsuche im Microsoft 365 Compliance Center verwenden, um Posteingangsregelereignisse anzuzeigen (Erstellen, Ändern und Löschen von Posteingangsregeln).

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Konfigurieren Sie auf der Registerkarte **"Suchen** " der **Überwachungsseite** die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich**: Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und **Ende** aus.
   - **Aktivitäten**: Wählen Sie einen oder mehrere der folgenden Werte aus:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Aktualisieren von Posteingangsregeln von Outlook Client**

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Wählen Sie eine Aktivität in den Ergebnissen aus, um das Detail-Flyout zu öffnen. Informationen zu den Posteingangsregeleinstellungen werden **im Parameterfeld** angezeigt.

Weitere Informationen finden Sie unter [Ermitteln, ob ein Benutzer eine Posteingangsregel erstellt hat](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
