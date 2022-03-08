---
title: Beispiel für eine Microsoft Defender für Office 365 Antiphishingrichtlinie
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
ms.openlocfilehash: 051823d9d7845550a1b707c55a1e1c970ebf6c32
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63206818"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Beispiel für eine Microsoft Defender für Office 365 Antiphishingrichtlinie

Diese Einstellungen aktivieren eine Richtlinie namens *"Domäne" und "CEO*". Diese Richtlinie bietet sowohl Benutzer- als auch Domänenschutz vor Identitätswechsel und wendet die Richtlinie dann auf alle E-Mails an, die von Benutzern innerhalb der Domäne empfangen werden. Fügen Sie zunächst die folgenden Informationen hinzu, um die Richtlinie zu erstellen:

- **Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.
  **Angewendet auf**: Wählen Sie **die Empfängerdomäne aus**. Wählen Sie unter **"Eine dieser** Elemente" die Option **"Auswählen"** aus, und wählen Sie dann eine Domäne aus. Wählen Sie **+ Hinzufügen** aus. Aktivieren Sie das Kontrollkästchen neben dem Namen der Domäne in der Liste (z. *B. contoso.com*), und wählen Sie dann **"Hinzufügen**" aus. Wählen Sie **Fertig** aus.
- Nachdem die Richtlinie erstellt wurde, können Sie die Richtlinie mit den folgenden Optionen optimieren:
  - **Hinzufügen von Benutzern zum Schutz:** Fügen Sie in diesem Beispiel mindestens die E-Mail-Adresse des CEO hinzu.
  - **Zu schützende Domänen hinzufügen**: Fügen Sie die Organisationsdomäne hinzu, die das Büro des CEO enthält.
  - **Wählen Sie Aktionen** aus: **Wenn E-Mails von einem imitierten Benutzer gesendet** werden, wählen Sie **"Nachricht an eine andere E-Mail-Adresse umleiten**" aus, und geben Sie dann die E-Mail-Adresse des Sicherheitsadministrators ein (z. *B. securityadmin@contoso.com*). For **If email is sent by an impersonated domain**, select **Quarantine the message**.
  - **Postfachintelligenz**: Diese Option ist standardmäßig aktiviert, wenn Sie eine neue Antiphishingrichtlinie erstellen. Lassen Sie diese Einstellung auf **Ein**, um optimale Ergebnisse zu erzielen.
  - **Fügen Sie vertrauenswürdige Absender und Domänen hinzu:** Definieren Sie in diesem Beispiel keine Außerkraftsetzungen.
- Nachdem Sie Ihre Einstellungen überprüft haben, wählen **Sie diese Richtlinie** erstellen oder **speichern** aus.

Weitere Informationen finden Sie [unter Antiphishingrichtlinien in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
