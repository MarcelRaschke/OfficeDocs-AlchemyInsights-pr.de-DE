---
title: Beheben der Sprach-/IP-Filterrichtlinie
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
ms.openlocfilehash: 25744bee6f3ed06ae67fc3c246c7d64fce9994bb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320524"
---
# <a name="fix-languageip-filter-policy"></a>Beheben der Sprach-/IP-Filterrichtlinie

Eine Ihrer Antispamrichtlinien wirkte sich auf diese Nachricht aus. Führen Sie die folgenden Schritte aus, um die Richtlinien zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail-& Richtlinien** für die Zusammenarbeit & Richtlinien für \>  \> **Bedrohungsregeln** \> **Antispam** im Abschnitt **"Richtlinien".**

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **"Antispamrichtlinien"** die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken (**Typ** ist **benutzerdefinierte Antispamrichtlinie** oder **Name** ist **Eingehende Antispamrichtlinie (Standard).**
3. Wählen Sie im angezeigten Flyout "Details" den **Spamschwellenwert und die Eigenschaften** bearbeiten im **Abschnitt "Massen-E-Mail-Schwellenwert & Spameigenschaften"** aus.
4. Überprüfen Sie im Abschnitt **"Als Spam markieren"** die Einstellungen **"Enthält bestimmte Sprachen"** und **"Aus diesen Ländern".**

Weitere Informationen finden Sie unter [Konfigurieren von Antispamrichtlinien in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
