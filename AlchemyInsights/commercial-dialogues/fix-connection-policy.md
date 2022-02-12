---
title: Beheben von Verbindungsrichtlinien
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
ms.openlocfilehash: d55b6a113600e5a967449c73ef9f90263504e9ee
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62656302"
---
# <a name="fix-connection-policy"></a>Beheben von Verbindungsrichtlinien

Die E-Mail wurde als sicher markiert und an den Posteingang des Benutzers übermittelt, da die Quell-IP-Adresse in der Standardverbindungsfilterrichtlinie als sicher markiert wurde. Führen Sie die folgenden Schritte aus, um die Richtlinie zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail und Zusammenarbeit** \> **Richtlinien und Regeln** \> **Bedrohungsrichtlinien** \> **Antispam** im Abschnitt **Richtlinien**.

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **"Antispamrichtlinien** " die Richtlinie namens **Verbindungsfilterrichtlinie (Standard)** aus, indem Sie auf den Namen der Richtlinie klicken.

3. Klicken Sie im angezeigten Flyout "Details" im Abschnitt **"Verbindungsfilterung"** auf " **Verbindungsfilterrichtlinie** bearbeiten".

4. Überprüfen Sie die Einträge im Abschnitt **"Nachrichten immer zulassen" aus dem folgenden Abschnitt "IP-Adressen" oder "Adressbereich** " und überprüfen Sie, ob " **Sichere Liste aktivieren** " ausgewählt ist.

   **Hinweis**: Microsoft abonniert Drittanbieterquellen vertrauenswürdiger Absender. Wenn die sichere Liste aktiviert ist, werden diese vertrauenswürdigen Absender nicht versehentlich als Spam gekennzeichnet. Wir empfehlen, diese Option auszuwählen, da dadurch die Anzahl falsch positiver Nachrichten (gute E-Mails, die als Spam klassifiziert werden) reduziert wird, die Sie erhalten.

Weitere Informationen finden Sie unter [Konfigurieren der Richtlinie für Verbindungsfilter](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
