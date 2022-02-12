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
ms.openlocfilehash: f8a913c9bbd98e8998dc65457e4acf666325e90c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62631174"
---
# <a name="teams-meeting-recordings-auto-expiration"></a>Automatisches Ablaufen von Microsoft Teams-Besprechungsaufzeichnungen

Ende März 2022 wird eine standardmäßige Ablaufeinstellung von 120 Tagen für alle **neu erstellten** Teams-Besprechungsaufzeichnungen (Teams Meeting Recordings, TMRs) ausgerollt. Diese Einstellung ist standardmäßig aktiviert und wirkt sich nicht auf vorhandene TMRs aus. Über PowerShell oder das Teams Admin Center können ein Teams-Administrator oder ein globaler Administrator [das Ablaufdatum ändern oder deaktivieren](https://docs.microsoft.com/MicrosoftTeams/meeting-expiration#change-the-default-expiration-date).

**Hinweis:** Einigen Kunden wird die Ablauf-Benutzeroberfläche in SharePoint/OneDrive möglicherweise vor dem Ablaufen von Microsoft Teams-Besprechungsaufzeichnungen angezeigt. In diesem Fall wird anstelle der Anzahl der Tage "Kein Ablauftermin" angezeigt. Dies bedeutet, dass diese Einstellung für Ihren Mandanten noch nicht vollständig ausgerollt ist. Suchen Sie im [Nachrichtencenter (MC274188)](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/MessageCenter) nach den aktuellsten Informationen zum Rolloutzeitplan.
