---
title: Beheben der Verbindungsrichtlinie
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
ms.openlocfilehash: d827ad73007fd4ffee374325f843ded6252f4735
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66414049"
---
# <a name="fix-connection-policy"></a>Beheben der Verbindungsrichtlinie

Die E-Mail wurde als sicher markiert und an den Posteingang des Benutzers übermittelt, da die Quell-IP-Adresse in der Standard-Verbindungsfilterrichtlinie als sicher gekennzeichnet wurde. Führen Sie die folgenden Schritte aus, um die Richtlinie zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail und Zusammenarbeit** \> **Richtlinien und Regeln** \> **Bedrohungsrichtlinien** \> **Antispam** im Abschnitt **Richtlinien**.

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **"Antispamrichtlinien** " die Richtlinie namens **"Verbindungsfilterrichtlinie" (Standard)** aus, indem Sie auf den Namen der Richtlinie klicken.

3. Klicken Sie im daraufhin angezeigten Flyout "Details" im Abschnitt "**Verbindungsfilterung**" auf "**Verbindungsfilterrichtlinie bearbeiten**".

4. Überprüfen Sie die Einträge im Abschnitt **"Nachrichten aus den folgenden IP-Adressen oder Adressbereichen immer zulassen** ", und überprüfen Sie, ob " **Sichere Liste aktivieren** " ausgewählt ist.

   **Hinweis**: Microsoft abonniert Drittanbieterquellen vertrauenswürdiger Absender. Wenn die Sichere Liste aktiviert ist, werden diese vertrauenswürdigen Absender nicht fälschlicherweise als Spam gekennzeichnet. Es wird empfohlen, diese Option auszuwählen, da dadurch die Anzahl falsch positiver Ergebnisse (gute E-Mails, die als Spam klassifiziert sind) reduziert wird, die Sie erhalten.

Weitere Informationen finden Sie unter [Konfigurieren der Richtlinie für Verbindungsfilter](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
