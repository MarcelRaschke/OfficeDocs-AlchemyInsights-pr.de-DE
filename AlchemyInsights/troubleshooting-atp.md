---
title: Problembehandlung Microsoft Defender für Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 1039
ms.date: 04/21/2020
ms.openlocfilehash: 11681f1ad0f0a4fce0e59d7faa1543aef7907319
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66360219"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Problembehandlung Microsoft Defender für Office 365

- **Bemerken Sie Verzögerungen bei der Zustellung von E-Mail-Nachrichten?** Erwägen Sie die Verwendung der [dynamischen Übermittlung](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#dynamic-delivery-in-safe-attachments-policies) in Ihren Richtlinien für sichere Anlagen. Mit dieser Aktion werden Verzögerungen bei der Zustellung von E-Mail-Nachrichten vermieden, während Empfänger vor schädlichen Dateien geschützt werden.
- **Möchten Sie falsch positive oder falsch negative Ergebnisse melden?** Verwenden Sie die Seite **"Übermittlungen**" im Microsoft 365 Defender Portal unter <https://sip.security.microsoft.com/reportsubmission?viewid=admin>.
- **Wussten Sie, dass Sie den Schutz sicherer Links für E-Mails aktivieren können, die zwischen Personen in Ihrer Organisation gesendet werden?** Führen Sie die folgenden Schritte aus:
  1. Wechseln Sie im Microsoft 365 Defender Portal unter <https://security.microsoft.com/>zu **"E-Mail & Zusammenarbeitsrichtlinien** \>  **& Richtlinien** für **Bedrohungsbedrohungen** \> für Regeln\>" im Abschnitt **"Richtlinien"**. Oder wechseln Sie direkt zu <https://security.microsoft.com/safelinksv2>.
  2. Führen Sie auf der Seite **"Sichere Links** " einen der folgenden Schritte aus:
     - **Neu**: Klicken Sie auf **"Erstellen** ", und rufen Sie die Seite **"Schutzeinstellungen"** des Richtlinienerstellungs-Assistenten auf.
     - **Ändern**: Wählen Sie eine vorhandene Richtlinie aus, indem Sie auf den Namen klicken. Führen Sie im daraufhin angezeigten Flyout "Details" den Abschnitt **"Schutzeinstellungen"** aus, und klicken Sie dann auf " **Schutzeinstellungen bearbeiten"**.
  3. Konfigurieren Sie auf der Seite **"Schutzeinstellungen"** die folgenden Einstellungen:
       - **Wählen Sie die Aktion für unbekannte potenziell böswillige URLs in Nachrichten** aus: Wählen Sie **"Ein**" aus.
       - Wählen Sie **"Sichere Links auf E-Mail-Nachrichten anwenden" aus, die innerhalb der Organisation gesendet werden**.
  4. Speichern Sie die Richtlinie, und lassen Sie bis zu 30 Minuten zeit, bis Ihre Änderungen angewendet werden.
