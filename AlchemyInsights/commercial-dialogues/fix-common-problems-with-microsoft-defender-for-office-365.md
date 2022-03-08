---
title: Beheben allgemeiner Probleme mit Microsoft Defender für Office 365
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
ms.openlocfilehash: c33b42f232da6534b7405321a990300115980ca5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63174019"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Beheben allgemeiner Probleme mit Microsoft Defender für Office 365

Hier sind einige Lösungen für häufige Probleme mit Microsoft Defender für Office 365:

- **Nachrichtenverzögerung**:

  Verzögerungen bei der E-Mail-Zustellung können durch Tresor Anlagenüberprüfung von Nachrichten verursacht werden. Weitere Informationen finden Sie unter [Tresor Richtlinieneinstellungen für Anlagen](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Melden falsch positiver oder negativer Ergebnisse**:

  Weitere Informationen finden Sie unter [Melden von Nachrichten und Dateien an Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Aktivieren Sie Tresor Linkschutz**:

  1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/>zu **E-Mail-& Richtlinien** für die Zusammenarbeit \> **& Richtlinien** **für Bedrohungsregeln** \> \> **Tresor Links** im Abschnitt **"Richtlinien**".

     To go directly to the **Tresor Links** page, use <https://security.microsoft.com/safelinksv2>.

  2. Wählen Sie auf der Seite **Tresor Links** die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken.
  3. Führen Sie im angezeigten Flyout "Details" einen der folgenden Schritte aus:
     - Um eine neue Richtlinie hinzuzufügen, wählen Sie **+Erstellen** aus. Ein Assistent wird gestartet, um Die Richtlinieneinstellungen zu definieren.
     - Um eine vorhandene Richtlinie zu bearbeiten, wählen Sie die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken. Wählen Sie im angezeigten Flyout "Details" im Abschnitt **"Schutzeinstellungen**" die Option **"Bearbeiten**" aus.
  4. Konfigurieren Sie auf der Seite **"Schutzeinstellungen** " die folgenden Einstellungen:
     - Aktivieren **Sie die Aktion für unbekannte potenziell schädliche URLs in Nachrichten**.
     - Wählen Sie **"Sichere Links auf innerhalb der Organisation gesendete Nachrichten anwenden**" aus.

  Weitere Informationen finden Sie unter ["Einrichten Tresor Links"-Richtlinien in Microsoft Defender für Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
