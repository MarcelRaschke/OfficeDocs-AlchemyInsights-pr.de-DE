---
title: Beispiel für eine Richtlinie für Microsoft Defender für Office 365 Tresor Anlagen
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988294"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Beispiel für eine Richtlinie für Microsoft Defender für Office 365 Tresor Anlagen

Diese Einstellungen aktivieren eine Richtlinie namens *"Keine Verzögerungen",* die Nachrichten sofort übermittelt und anlagen nach der Überprüfung erneut angibt:

- **Name:** Keine Verzögerungen
- **Beschreibung:** Übermittelt Nachrichten sofort und fügt Anlagen nach der Überprüfung erneut an.
- **Antwort:** Wählen Sie die Option **"Dynamische Zustellung"** aus. Weitere Informationen finden Sie unter ["Dynamische Zustellung" in Tresor Anlagenrichtlinien.](https://go.microsoft.com/fwlink/?linkid=2092328)
- Abschnitt **"Anlage umleiten":** Wählen Sie die Option zum Aktivieren der **Umleitung** aus, und geben Sie dann die E-Mail-Adresse Ihres Microsoft 365 globalen Administrators, Sicherheitsadministrators oder Sicherheitsanalysten ein, der böswillige Anlagen untersuchen wird.
- **Angewendet auf** Abschnitt: Wählen Sie **die Empfängerdomäne aus,** und wählen Sie dann Ihre Domäne aus. Wählen Sie **"Hinzufügen"** und dann **"OK"** aus. Sobald Sie fertig sind, wählen Sie **Speichern** aus.

Weitere Informationen finden Sie [unter Tresor Anlagen in Microsoft Defender für Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
