---
title: Verwenden von Giphys in Teams-Unterhaltungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: d096113995ec9a13be695fd50e7c917aae1b8ed9
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66527196"
---
# <a name="using-giphys-in-teams-conversations"></a>Verwenden von Giphys in Teams-Unterhaltungen

Der Giphys-Zugriff im Teams-Chat ist standardmäßig aktiviert. Als Administrator können Sie steuern, ob Giphys für Benutzer verfügbar ist, indem [Sie eine Messagingrichtlinie festlegen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) und sicherstellen, dass **die Verwendung von Giphys in Unterhaltungen** **aktiviert** ist.

Wenn GIFs in Teams-Unterhaltungen nicht wie erwartet funktionieren, überprüfen Sie Folgendes:

Die [Messaging-Richtlinie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muss Giphys zulassen. So überprüfen Sie die Überprüfung mithilfe von PowerShell-Cmdlets:

- Stellen Sie sicher, dass Sie [Teams mit PowerShell verwalten](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#manage-teams-with-powershell) können.
- Führen Sie den PowerShell-Befehl [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps&preserve-view=true) aus, und stellen Sie sicher, dass **AllowGiphy** auf **TRUE** festgelegt ist.
- Wenn **AllowGiphy** auf **FALSE** festgelegt ist, führen Sie den folgenden PowerShell-Befehl [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps&preserve-view=true) aus.

[Optionale verbundene Erfahrungen](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) müssen aktiviert sein, um den Zugriff auf die Giphy-URL zu ermöglichen.

**Hinweis**: Wenn Sie mehrere Teams-Messagingrichtlinien für Ihren Mandanten konfiguriert haben, können Sie die Identität der Richtlinie bestimmen, die dem betroffenen Benutzer zugewiesen ist, mit dem PowerShell-Befehl ["Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps&preserve-view=true) \<user@domain.com\> | Wählen Sie "TeamsMessagingPolicy" aus.
