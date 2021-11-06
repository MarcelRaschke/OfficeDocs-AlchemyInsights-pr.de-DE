---
title: Problembehandlung bei Microsoft Defender für Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 1b441a14faafe0757f36647a935c4938c3c21139
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799110"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Problembehandlung bei Microsoft Defender für Office 365

- **Beachten Sie Verzögerungen bei der Zustellung von E-Mail-Nachrichten?** Erwägen Sie die Verwendung der [dynamischen Zustellung](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#dynamic-delivery-in-safe-attachments-policies) in Ihren Tresor Anlagenrichtlinien. Mit dieser Aktion werden Verzögerungen bei der Zustellung von E-Mails vermieden, während Empfänger vor schädlichen Dateien geschützt werden.
- **Möchten Sie falsch positive oder falsch negative Ergebnisse melden?** Verwenden Sie die Seite **"Übermittlungen"** im Microsoft 365 Defender Portal unter <https://sip.security.microsoft.com/reportsubmission?viewid=admin> .
- **Wissen Sie, dass Sie Tresor Linksschutz für E-Mails aktivieren können, die zwischen Personen in Ihrer Organisation gesendet werden?** Führen Sie die folgenden Schritte aus:
  1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> **"E-Mail-&** \> **Zusammenarbeitsrichtlinien & Bedrohungsrichtlinien** für Regeln \>  \> **Tresor Links"** im Abschnitt **"Richtlinien".** Oder wechseln Sie direkt zu <https://security.microsoft.com/safelinksv2> .
  2. Führen Sie auf der Seite **Tresor Links** einen der folgenden Schritte aus:
     - **Neu:** Klicken Sie auf **"Erstellen",** und rufen Sie die Seite **"Schutzeinstellungen"** des Assistenten zum Erstellen von Richtlinien auf.
     - **Ändern:** Wählen Sie eine vorhandene Richtlinie aus, indem Sie auf den Namen klicken. In the details flyout that appears, fin the **Protection settings** section, and then click Edit **protection settings**.
  3. Konfigurieren Sie auf der Seite **"Schutzeinstellungen"** die folgenden Einstellungen:
       - **Wählen Sie die Aktion für unbekannte potenziell schädliche URLs in Nachrichten** aus: **Aktivieren**.
       - Wählen Sie **"Anwenden Tresor Links auf E-Mail-Nachrichten, die innerhalb der Organisation gesendet werden"** aus.
  4. Speichern Sie die Richtlinie, und lassen Sie bis zu 30 Minuten zu, bis Ihre Änderungen übernommen werden.
