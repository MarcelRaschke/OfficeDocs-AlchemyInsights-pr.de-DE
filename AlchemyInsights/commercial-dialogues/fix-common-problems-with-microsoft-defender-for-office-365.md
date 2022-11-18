---
title: Beheben häufiger Probleme mit Microsoft Defender für Office 365
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
ms.openlocfilehash: 034f618ee11f9405dbfba27acd92f84c94139450
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66515532"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Beheben häufiger Probleme mit Microsoft Defender für Office 365

Hier sind einige Lösungen für häufige Probleme mit Microsoft Defender für Office 365:

- **Nachrichtenverzögerung**:

  Verzögerungen bei der Zustellung von E-Mails können durch das Scannen sicherer Anlagen von Nachrichten verursacht werden. Weitere Informationen finden Sie unter [Richtlinieneinstellungen für sichere Anlagen](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Falsch positive oder negative Ergebnisse melden**:

  Weitere Informationen finden Sie unter [Melden von Nachrichten und Dateien an Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Schutz sicherer Links aktivieren**:

  1. Wechseln Sie im Microsoft 365 Defender Portal unter <https://security.microsoft.com/>zu **"E-Mail & Zusammenarbeitsrichtlinien** \>  **& Richtlinien** für **Bedrohungsbedrohungen** \> für Regeln\>" im Abschnitt **"Richtlinien"**.

     Um direkt zur Seite " **Sichere Links"** zu wechseln, verwenden Sie <https://security.microsoft.com/safelinksv2>.

  2. Wählen Sie auf der Seite **"Sichere Links** " die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken.
  3. Führen Sie im daraufhin angezeigten Detailflyout einen der folgenden Schritte aus:
     - Um eine neue Richtlinie hinzuzufügen, wählen Sie **+Erstellen** aus. Ein Assistent wird gestartet, der Ihnen beim Definieren Ihrer Richtlinieneinstellungen hilft.
     - Um eine vorhandene Richtlinie zu bearbeiten, wählen Sie die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken. Wählen Sie im daraufhin angezeigten Flyout "Details" im Abschnitt **"Schutzeinstellungen**" die Option **"Bearbeiten**" aus.
  4. Konfigurieren Sie auf der Seite **"Schutzeinstellungen"** die folgenden Einstellungen:
     - Aktivieren **Sie "Aktion für unbekannte potenziell böswillige URLs in Nachrichten auswählen**".
     - Wählen Sie **"Sichere Links auf Innerhalb der Organisation gesendete Nachrichten anwenden**" aus.

  Weitere Informationen finden Sie unter [Einrichten von Richtlinien für sichere Links in Microsoft Defender für Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
