---
title: Probleme beim Erstellen von Live-Ereignissen in Yammer
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: d8c08cce2699b4bf4ccd77a93b1cf8fd0d1a0fdd
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63283913"
---
# <a name="live-events-in-yammer-creation-errors"></a>Probleme beim Erstellen von Live-Ereignissen in Yammer

**Erstellen von Live-Ereignissen in Yammer**

In Yammer wird jederzeit die Option zum Erstellen eines Live-Ereignisses angezeigt. In einigen Fällen erfüllt ein Benutzer möglicherweise nicht die Voraussetzungen für die Erstellung eines Live-Ereignisses und erhält eine Fehlermeldung, wenn er versucht, ein Live-Ereignis zu erstellen. Die folgenden Elemente behandeln häufige Ursachen für dieses Problem und bieten Möglichkeiten zur Behebung des Problems für Endbenutzer.

**Wer kann Liveereignisse erstellen**
- Eine Lizenz für Office 365 Enterprise E1, E3 oder E5 oder eine Lizenz für Office 365 A3 oder A5.
- Die Berechtigung zum Erstellen von Live-Ereignissen im Microsoft Teams Admin Center.
- Die Berechtigung zum Erstellen von Live Ereignissen in Microsoft Stream (für Ereignisse, die mit einer externen Broadcasting-App oder einem externen Gerät erstellt wurden).
- Vollständige Teammitgliedschaft in der Organisation (darf kann kein Gast oder jemand von einer anderen Organisation sein)
- Planung von privaten Besprechungen, Screensharing und IP-Videofreigabe – in der Team-Besprechungsrichtlinie aktiviert.

**Richtlinien zur Erstellung von Liveereignissen**

Yammer folgt den Richtlinien für Live-Ereignisse, die in Ihrem Office 365-Mandanten für Stream festgelegt sind. Standardmäßig kann jeder in Ihrer Organisation ein Live-Event erstellen. Administratoren können [möglicherweise Änderungen an dieser Einstellung vornehmen, wodurch Benutzer daran gehindert werden, ein Live Ereignis zu erstellen](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating). Es ist wichtig, zu überprüfen, ob die Benutzer über die Berechtigung zum Erstellen von Live-Ereignissen verfügen, wenn sie einen Richtlinienfehler erhalten.
