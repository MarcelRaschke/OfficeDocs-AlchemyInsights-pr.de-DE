---
title: Beispiel für Microsoft Defender für Office 365 Richtlinie für sichere Anlagen
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
ms.openlocfilehash: 0bd61b58fde77f6c74cc6dbdfa3d737612c9ed7d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66326428"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Beispiel für Microsoft Defender für Office 365 Richtlinie für sichere Anlagen

Mit diesen Einstellungen wird eine Richtlinie namens *"Keine Verzögerungen* " aktiviert, die Nachrichten sofort übermittelt, und anlagen nach dem Scannen erneut anordnen:

- **Name**: Keine Verzögerungen
- **Beschreibung**: Nachrichten werden sofort übermittelt und Anlagen nach dem Scannen erneut angefügt.
- **Antwort**: Wählen Sie die Option **"Dynamische Übermittlung** " aus. Weitere Informationen finden Sie [unter Dynamische Zustellung in Richtlinien für sichere Anlagen](https://go.microsoft.com/fwlink/?linkid=2092328).
- Abschnitt "**Anlage umleiten**": Wählen Sie die Option zum **Aktivieren der Umleitung** aus, und geben Sie dann die E-Mail-Adresse Ihres globalen Microsoft 365-Administrators, Sicherheitsadministrators oder Sicherheitsanalysten ein, der schädliche Anlagen untersucht.
- **Abschnitt "Angewendet auf** ": Wählen Sie **"Empfängerdomäne"** aus, und wählen Sie dann Ihre Domäne aus. Wählen Sie **"Hinzufügen"** und dann **"OK**" aus. Sobald Sie fertig sind, wählen Sie **"Speichern"** aus.

Weitere Informationen finden Sie [unter "Sichere Anlagen" in Microsoft Defender für Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
