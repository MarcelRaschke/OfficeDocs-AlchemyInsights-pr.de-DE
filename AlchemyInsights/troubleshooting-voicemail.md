---
title: 'Problembehandlung für Voicemail '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: d2fb4d9e3dc869acf0201e86402357dd08d88283
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63196808"
---
# <a name="troubleshooting-voicemail"></a>Problembehandlung für Voicemail

Stellen Sie sicher, dass die Funktion "Besetzt bei Gebucht" beabsichtigt ist.

Wenn dieses Feature für diesen Benutzer nicht benötigt wird:

1. Wechseln Sie zu [Teams Admin Center](https://admin.teams.microsoft.com/policies/calling).
1. Navigieren Sie auf der linken Leiste zu **"VoiceCalling** >  **policiesManage** >  Policies" in der **Anrufrichtlinie**.
1. Wählen Sie **"Benutzer verwalten" aus**.
1. Suchen Sie nach einem Benutzer, und ändern Sie die Anrufrichtlinie in eine Richtlinie, die beschäftigt **ist, ist verfügbar, wenn sie in einem Anruf** von **"Aus" aufgerufen wird**.
1. Klicken Sie auf **Anwenden**.

**Hinweis**: Es kann bis zu 24 Stunden dauern, bis Änderungen an Richtlinien repliziert wurden.

Weitere Informationen zu diesem Feature finden Sie unter: [Beschäftigt bei Gebucht ist während eines Anrufs verfügbar](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
