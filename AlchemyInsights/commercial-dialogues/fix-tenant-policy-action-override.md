---
title: Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326796"
---
# <a name="fix-tenant-policy-action-override"></a>Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)

Eine Ihrer Antispamrichtlinien wirkte sich auf diese Nachricht aus. Führen Sie die folgenden Schritte aus, um die Richtlinien zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail-& Richtlinien** für die Zusammenarbeit & Richtlinien für \>  \> **Bedrohungsregeln** \> **Antispam** im Abschnitt **"Richtlinien".**

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **"Antispamrichtlinien"** die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken (**Typ** ist **benutzerdefinierte Antispamrichtlinie** oder **Name** ist **Eingehende Antispamrichtlinie (Standard).**
3. Wählen Sie im angezeigten Flyout "Details" die **Option "Aktionen bearbeiten"** im Abschnitt **"Aktionen"** aus.
4. Überprüfen Sie im Abschnitt **"Nachrichtenaktionen"** die Bewertungen für **Spam,** **Spam mit hoher Spamwahrscheinlichkeit,** **Phishing** und Phishing mit **hoher Vertrauenswürdigkeit,** um festzustellen, ob einer der folgenden Werte ausgewählt ist:
   - **X-Header hinzufügen**
   - **Text in Betreffzeile voranstellen**
   - **Nachricht an E-Mail-Adresse umleiten**
   - **Nachricht löschen**
   - **Keine Aktion**

   Es ist möglich, dass die **Standardeinstellungen,** die auf alle Exchange Online Protection Kunden angewendet wurden, die Nachricht betroffen sind.

Weitere Informationen finden Sie unter [Konfigurieren von Antispamrichtlinien in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
