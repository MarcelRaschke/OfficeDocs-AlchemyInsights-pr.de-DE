---
title: Beispiel für eine Microsoft Defender für Office 365 Antiphishingrichtlinie
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035005"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Beispiel für eine Microsoft Defender für Office 365 Antiphishingrichtlinie

Diese Einstellungen aktivieren eine Richtlinie namens *"Domäne" und "CEO".* Diese Richtlinie bietet sowohl Benutzer- als auch Domänenschutz vor Identitätswechsel und wendet die Richtlinie dann auf alle E-Mails an, die von Benutzern innerhalb der Domäne empfangen werden. Fügen Sie zunächst die folgenden Informationen hinzu, um die Richtlinie zu erstellen:

- **Name**: Domain and CEO **Description**: Stellt sicher, dass der CEO und Ihre Domäne nicht imitiert werden.
  **Angewendet auf:** Wählen Sie **die Empfängerdomäne aus.** Wählen Sie unter **Eine dieser** Elemente die Option **Auswählen** und dann Domäne aus. Wählen Sie **+ Hinzufügen** aus. Aktivieren Sie das Kontrollkästchen neben dem Namen der Domäne in der Liste (z. *B. contoso.com*), und wählen Sie dann **Hinzufügen** aus. Wählen Sie **Fertig** aus.
- Nachdem die Richtlinie erstellt wurde, können Sie die Richtlinie mit den folgenden Optionen optimieren:
  - **Hinzufügen von Benutzern zum Schutz:** Fügen Sie in diesem Beispiel mindestens die E-Mail-Adresse des CEO hinzu.
  - **Hinzufügen von Domänen zum Schutz:** Fügen Sie die Organisationsdomäne hinzu, die das Büro des CEO enthält.
  - **Wählen Sie Aktionen** aus: **Wenn E-Mails von einem imitierten Benutzer gesendet** werden, wählen Sie **"Nachricht an eine andere E-Mail-Adresse umleiten"** aus, und geben Sie dann die E-Mail-Adresse des Sicherheitsadministrators ein (z. *B. securityadmin@contoso.com*). For **If email is sent by an impersonated domain**, select Quarantine the **message**.
  - **Postfachintelligenz:** Diese Option ist standardmäßig aktiviert, wenn Sie eine neue Antiphishingrichtlinie erstellen. Lassen Sie diese Einstellung auf **Ein**, um optimale Ergebnisse zu erzielen.
  - **Fügen Sie vertrauenswürdige Absender und Domänen hinzu:** Definieren Sie in diesem Beispiel keine Außerkraftsetzungen.
- Nachdem Sie Ihre Einstellungen überprüft haben, wählen **Sie diese Richtlinie** erstellen oder **speichern** aus.

Weitere Informationen finden Sie [unter Antiphishingrichtlinien in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
