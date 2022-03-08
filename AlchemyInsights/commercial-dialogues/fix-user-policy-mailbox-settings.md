---
title: Korrigieren von Benutzerrichtlinien-/Postfacheinstellungen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9c6d36fe128af9cce47dffd5ff52e00a0e1a181e
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63241073"
---
# <a name="fix-user-policymailbox-settings"></a>Korrigieren von Benutzerrichtlinien-/Postfacheinstellungen

Die Junk-E-Mail-Einstellungen für das Postfach haben diese Nachricht beeinflusst. Gehen Sie folgendermaßen vor, um die Einstellungen zu überprüfen:

1. Starten Sie Exchange Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Führen Sie diesen Befehl aus (unter Verwendung der  **E-Mail-Adresse des Benutzers): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Überprüfen Sie, ob die E-Mail-Adresse des Absenders Teil von **TrustedSendersAndDomains** oder **BlockedSendersAndDomains** ist. Wenn sich die E-Mail-Adresse in einer der Listen befindet, müssen Sie sie möglicherweise entfernen. Weitere Informationen finden Sie unter ["Set-MailboxJunkEmailConfiguration"](https://go.microsoft.com/fwlink/?linkid=2101047).
