---
title: Meldung „Keine Abonnements gefunden“ im Security Center
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9001222"
- "6028"
ms.date: 07/16/2020
ms.openlocfilehash: b10ab5a45aa0c22b2e9aba2155e2a3e11e736096
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66387597"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Meldung „Keine Abonnements gefunden“ im Security Center

Wenn Sie beim Zugriff auf das Microsoft Defender Security Center die Meldung „Keine Abonnements gefunden“ erhalten, bedeutet dies, dass das Azure Active Directory (AAD), mit dem sich der Benutzer am Portal anmeldet, keine Microsoft Defender ATP-Lizenz hat.  

Die Lizenzen für Windows E5 und Office E5 sind separate Lizenzen.

Öffnen Sie einen Supportfall, wenn die Lizenz erworben, aber nicht für diese AAD-Instanz bereitgestellt wurde. Sie verfügen entweder über: <br/>
-   ein mögliches Problem bei der Lizenzbereitstellung auf.<br/>
-   Oder Sie haben die Lizenz versehentlich für ein anderes Microsoft AAD als das für die Authentifizierung beim Dienst verwendete bereitgestellt.