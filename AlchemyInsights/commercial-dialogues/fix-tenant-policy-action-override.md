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
ms.openlocfilehash: d34b002a4e6e3ec510226d963e3621ba1f3409fa
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62656122"
---
# <a name="fix-tenant-policy-action-override"></a>Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)

Eine Ihrer Antispamrichtlinien wirkte sich auf diese Nachricht aus. Führen Sie die folgenden Schritte aus, um die Richtlinien zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail und Zusammenarbeit** \> **Richtlinien und Regeln** \> **Bedrohungsrichtlinien** \> **Antispam** im Abschnitt **Richtlinien**.

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **Antispamrichtlinien** die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken (**Type** ist **Benutzerdefinierte Antispamrichtlinie** oder **Name** ist **Antispam-Eingangsrichtlinie (Standard)**).
3. Wählen Sie im angezeigten Flyout "Details" die **Option "Aktionen bearbeiten** " im Abschnitt **"Aktionen"** aus.
4. Überprüfen Sie im Abschnitt " **Nachrichtenaktionen** " die Bewertungen für **Spam**, **Spam mit hoher Spamwahrscheinlichkeit**, **Phishing** und **Phishing mit hoher Vertrauenswürdigkeit** , um festzustellen, ob einer der folgenden Werte ausgewählt ist:
   - **X-Header hinzufügen**
   - **Text in Betreffzeile voranstellen**
   - **Nachricht an E-Mail-Adresse umleiten**
   - **Nachricht löschen**
   - **Keine Aktion**

   Es ist möglich, dass die **Standardeinstellungen** auf alle Exchange Online Protection Kunden angewendet wurden, die die Nachricht betroffen haben.

Weitere Informationen finden Sie unter [Konfigurieren von Antispamrichtlinien in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
