---
title: Verwenden von Giphys in Teams Unterhaltungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 1e1f417280da1e350c736daa3ee7d82909ad3e70
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62740583"
---
# <a name="using-giphys-in-teams-conversations"></a>Verwenden von Giphys in Teams Unterhaltungen

Der Giphys-Zugriff in Teams Chat ist standardmäßig aktiviert. Als Administrator können Sie steuern, ob Giphys für Benutzer verfügbar ist, indem Sie [eine Messagingrichtlinie festlegen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) und sicherstellen, dass **Giphys in Unterhaltungen** **verwendet wird.**

Wenn GIFs in Teams Unterhaltungen nicht wie erwartet funktionieren, überprüfen Sie Folgendes:

Die [Messaging-Richtlinie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muss Giphys zulassen. So überprüfen Sie dies mithilfe von PowerShell-Cmdlets:

- Stellen Sie sicher, dass Sie [Teams mit PowerShell verwalten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#manage-teams-with-powershell) können.
- Führen Sie den [PowerShell-Befehl Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps&preserve-view=true) aus, und stellen Sie sicher, dass **AllowGiphy** auf **TRUE** festgelegt ist.
- Wenn **AllowGiphy** auf **FALSE** festgelegt ist, führen Sie den folgenden [PowerShell-Befehl Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps&preserve-view=true) aus.

[Optionale verbundene Erfahrungen](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) müssen aktiviert sein, um den Zugriff auf die Giphy-URL zu ermöglichen.

**Hinweis**: Wenn Sie mehrere Teams Messagingrichtlinien für Ihren Mandanten konfiguriert haben, können Sie die Identität der Richtlinie ermitteln, die dem betroffenen Benutzer mit dem [PowerShell-Befehl Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps&preserve-view=true) \<user@domain.com\> | Wählen Sie "TeamsMessagingPolicy" aus.
