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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323519"
---
# <a name="using-giphys-in-teams-conversations"></a>Verwenden von Giphys in Teams Unterhaltungen

Der Giphys-Zugriff in Teams Chat ist standardmäßig aktiviert. Als Administrator können Sie steuern, ob Giphys für Benutzer verfügbar ist, indem Sie [eine Messagingrichtlinie festlegen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) und sicherstellen, dass **Giphys in Unterhaltungen** verwendet **wird.**

Wenn GIFs in Teams Unterhaltungen nicht wie erwartet funktionieren, überprüfen Sie:

Die [Messaging-Richtlinie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muss Giphys zulassen. So überprüfen Sie dies mithilfe von PowerShell-Cmdlets:

- Stellen Sie sicher, dass Sie [Teams mit PowerShell verwalten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)können.
- Führen Sie den [PowerShell-Befehl Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) aus, und stellen Sie sicher, dass **AllowGiphy** auf **TRUE** festgelegt ist.
- Wenn **AllowGiphy** auf **FALSE** festgelegt ist, führen Sie den folgenden [PowerShell-Befehl Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)aus.

[Optionale verbundene Erfahrungen](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) müssen aktiviert sein, um den Zugriff auf die Giphy-URL zu ermöglichen.

**Hinweis:** Wenn Sie mehrere Teams Messagingrichtlinien für Ihren Mandanten konfiguriert haben, können Sie die Identität der Richtlinie ermitteln, die dem betroffenen Benutzer mit dem [PowerShell-Befehl Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Wählen Sie "TeamsMessagingPolicy" aus.
