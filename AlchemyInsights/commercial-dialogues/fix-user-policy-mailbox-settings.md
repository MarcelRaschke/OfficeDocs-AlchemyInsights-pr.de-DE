---
title: Korrigieren von Benutzerrichtlinien-/Postfacheinstellungen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034717"
---
# <a name="fix-user-policymailbox-settings"></a>Korrigieren von Benutzerrichtlinien-/Postfacheinstellungen

Die Junk-E-Mail-Einstellungen für das Postfach haben diese Nachricht beeinflusst. Gehen Sie folgendermaßen vor, um die Einstellungen zu überprüfen:

1. Starten Sie Exchange Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Führen Sie diesen Befehl aus (mithilfe der E-Mail-Adresse des Benutzers):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Überprüfen Sie, ob die E-Mail-Adresse des Absenders Teil von **TrustedSendersAndDomains** oder **BlockedSendersAndDomains** ist. Wenn sich die E-Mail-Adresse in einer der Listen befindet, müssen Sie sie möglicherweise entfernen. Weitere Informationen finden Sie unter ["Set-MailboxJunkEmailConfiguration".](https://go.microsoft.com/fwlink/?linkid=2101047)
