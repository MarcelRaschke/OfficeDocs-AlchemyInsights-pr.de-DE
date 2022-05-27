---
title: Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach
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
- "3100008"
- "7217"
ms.openlocfilehash: b6faa07a40ae234db51b03a97982485b193cddd7
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65727244"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach

Hier erfahren Sie, wie Sie eine Richtlinie einrichten, mit der die alten E-Mails eines Benutzers automatisch in das Archivpostfach verschoben werden:

1. Wechseln Sie zu [**"Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data Governance** > **Archive** ", um zu überprüfen, ob ein Archivpostfach für den Benutzer aktiviert wurde. Falls nicht, klicken Sie im Warnfeld auf **"Aktivieren** " und dann auf " **Ja** ".
2. Wechseln Sie zu [**Exchange Admin Center > Complianceverwaltung > Aufbewahrungstags**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Wählen Sie das +-Symbol und dann **"Automatisch auf das gesamte Postfach anwenden**" aus.
4. Weisen Sie dem Aufbewahrungstag einen Namen zu, und wählen Sie **"In Archiv verschieben"** aus. Geben Sie für den Aufbewahrungszeitraum die gewünschte Zeit ein, z. B. 90 Tage. Klicken Sie auf **Speichern**.
5. Erstellen Sie jetzt eine Aufbewahrungsrichtlinie: Wählen Sie **"Aufbewahrungsrichtlinien**" und dann das Symbol aus, um eine neue Richtlinie hinzuzufügen.
6. Weisen Sie der Aufbewahrungsrichtlinie einen Namen zu, klicken Und scrollen Sie dann, um das soeben erstellte Aufbewahrungstag zu suchen und hinzuzufügen. Klicken Sie auf **Speichern**.
7. Wenden Sie schließlich die Aufbewahrungsrichtlinie auf das Postfach des Benutzers an: Wechseln Sie im Exchange Admin Center zu **den Empfängerpostfächern** > . Wählen Sie alle Benutzer aus, auf die Sie die Richtlinie anwenden möchten, und wählen Sie dann **"Bearbeiten"** (das Stiftsymbol) aus.
8. Klicken Sie im Dialogfeld auf **"Postfachfeatures"**. Wenden Sie unter **"Aufbewahrungsrichtlinie"** die Richtlinie an, die Sie soeben > **Speichern** erstellt haben.
9. Anweisungen zum Anwenden der Richtlinie auf alle Benutzer finden Sie unter [Anwenden einer Aufbewahrungsrichtlinie auf Postfächer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
