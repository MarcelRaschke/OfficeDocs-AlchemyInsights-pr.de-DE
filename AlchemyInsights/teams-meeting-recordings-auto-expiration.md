---
title: Automatisches Ablaufen von Microsoft Teams-Besprechungsaufzeichnungen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "13757"
- "9002530"
ms.date: 01/21/2022
ms.openlocfilehash: 09d27855fceedc51bacced22ad54c43bbe5b44b8
ms.sourcegitcommit: 5dcbecdebbf5042db0c86a12149ddd537d766c91
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2022
ms.locfileid: "62185132"
---
# <a name="teams-meeting-recordings-auto-expiration"></a>Automatisches Ablaufen von Microsoft Teams-Besprechungsaufzeichnungen

Wir führen eine Standard-Ablauffrist von 60 Tagen für alle neu erstellten Microsoft Teams-Besprechungsaufzeichnungen ein. Die entsprechende Einstellung ist standardmäßig aktiviert und wirkt sich nicht auf vorhandene Aufzeichnungen aus. Wenn ein Administrator [die Ablauffrist ändern oder deaktivieren](https://docs.microsoft.com/MicrosoftTeams/meeting-expiration#change-the-default-expiration-date) möchte, kann er dies über PowerShell oder das Microsoft Teams Admin Center tun.

**Hinweis:** Einigen Kunden wird die Ablauf-Benutzeroberfläche in SharePoint/OneDrive möglicherweise vor dem Ablaufen von Microsoft Teams-Besprechungsaufzeichnungen angezeigt. In diesem Fall wird anstelle der Anzahl der Tage "Kein Ablauftermin" angezeigt. Dies bedeutet, dass das Rollout dieser Einstellung für Ihren Mandanten noch nicht vollständig abgeschlossen ist. Suchen Sie im [Nachrichtencenter (MC274188)](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/MessageCenter) nach den aktuellsten Informationen zum Rolloutzeitplan.
