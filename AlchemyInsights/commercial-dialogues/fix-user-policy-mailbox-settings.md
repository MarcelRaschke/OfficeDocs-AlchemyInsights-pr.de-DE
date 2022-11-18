---
title: Beheben von Benutzerrichtlinien-/Postfacheinstellungen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fb4f910800d77497c717593b90af35f6c8602620
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66380325"
---
# <a name="fix-user-policymailbox-settings"></a>Beheben von Benutzerrichtlinien-/Postfacheinstellungen

Die Junk-E-Mail-Einstellungen im Postfach wirkten sich auf diese Nachricht aus. Gehen Sie wie folgt vor, um die Einstellungen zu überprüfen:

1. Starten Sie die Exchange-Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Führen Sie diesen Befehl aus (mithilfe der E-Mail-Adresse des Benutzers):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Überprüfen Sie, ob die E-Mail-Adresse des Absenders Teil von **TrustedSendersAndDomains** oder **BlockedSendersAndDomains** ist. Wenn sich die E-Mail-Adresse in einer der Listen befindet, müssen Sie sie möglicherweise entfernen. Weitere Informationen finden Sie unter [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
