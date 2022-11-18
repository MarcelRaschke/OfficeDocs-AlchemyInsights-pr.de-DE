---
title: Beispiel für Microsoft Defender für Office 365 Antiphishingrichtlinie
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
ms.openlocfilehash: 01021c7906e05bcc72be06d322245e9b975ced96
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66326487"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Beispiel für Microsoft Defender für Office 365 Antiphishingrichtlinie

Diese Einstellungen aktivieren eine Richtlinie namens *"Domäne und CEO"*. Diese Richtlinie bietet sowohl Benutzer- als auch Domänenschutz vor Identitätswechsel und wendet die Richtlinie dann auf alle E-Mails an, die von Benutzern innerhalb der Domäne empfangen werden. Fügen Sie zunächst die folgenden Informationen hinzu, um die Richtlinie zu erstellen:

- **Name**: Domänen- und **CEO-Beschreibung**: Stellt sicher, dass der CEO und Ihre Domäne nicht imitiert werden.
  **Angewendet auf**: Wählen Sie **die Empfängerdomäne aus**. Wählen Sie unter **"Eine dieser** Optionen" die Option **"Auswählen"** aus, und wählen Sie dann eine Domäne aus. Wählen Sie **+ Hinzufügen** aus. Aktivieren Sie das Kontrollkästchen neben dem Namen der Domäne in der Liste (z. B *. contoso.com*), und wählen Sie dann **"Hinzufügen"** aus. Wählen Sie **Fertig** aus.
- Nachdem die Richtlinie erstellt wurde, können Sie die Richtlinie mithilfe der folgenden Optionen optimieren:
  - **Benutzer zum Schutz hinzufügen:** Fügen Sie in diesem Beispiel mindestens die E-Mail-Adresse des CEO hinzu.
  - **Zu schützenden Domänen hinzufügen**: Fügen Sie die Organisationsdomäne hinzu, die das Büro des CEO enthält.
  - **Auswählen von Aktionen**: **Wenn E-Mails von einem imitierten Benutzer gesendet** werden, wählen Sie **"Nachricht an eine andere E-Mail-Adresse umleiten**" aus, und geben Sie dann die E-Mail-Adresse des Sicherheitsadministrators ein (z. B *. securityadmin@contoso.com*). For **If email is sent by an impersonated domain**, select **Quarantine the message**.
  - **Postfachintelligenz**: Standardmäßig ist diese Option ausgewählt, wenn Sie eine neue Antiphishingrichtlinie erstellen. Lassen Sie diese Einstellung auf **Ein**, um optimale Ergebnisse zu erzielen.
  - **Vertrauenswürdige Absender und Domänen hinzufügen:** Definieren Sie in diesem Beispiel keine Außerkraftsetzungen.
- Nachdem Sie Ihre Einstellungen überprüft haben, wählen **Sie nach Bedarf "Diese Richtlinie erstellen** " oder " **Speichern"** aus.

Weitere Informationen finden Sie [unter Antiphishingrichtlinien in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
