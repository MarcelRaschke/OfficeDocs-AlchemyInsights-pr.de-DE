---
title: Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach
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
- "3100008"
- "7217"
ms.openlocfilehash: 896cc2fa4f9a83e09cb40cbbc55ba747b1520639
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62672899"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach

Hier erfahren Sie, wie Sie eine Richtlinie einrichten, um die alte E-Mail eines Benutzers automatisch in das Archivpostfach zu verschieben:

1. Wechseln Sie zu [**Security & ComplianceData**](https://go.microsoft.com/fwlink/p/?linkid=2077143) >  **governanceArchive** > , um zu überprüfen, ob ein Archivpostfach für den Benutzer aktiviert wurde. Wenn dies nicht der Fall ist, klicken Sie im Warnfeld auf **"Aktivieren** ", dann auf **"Ja** ".
2. Wechseln Sie zu [**Exchange Admin Center > Complianceverwaltung > Aufbewahrungstags**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Wählen Sie das Symbol +, und klicken Sie dann automatisch **auf das gesamte Postfach anwenden**.
4. Weisen Sie dem Aufbewahrungstag einen Namen zu, und wählen Sie **"In Archiv verschieben**" aus. Geben Sie für den Aufbewahrungszeitraum die gewünschte Zeit ein, z. B. 90 Tage. Klicken Sie auf **Speichern**.
5. Erstellen Sie nun eine Aufbewahrungsrichtlinie: Wählen Sie **Aufbewahrungsrichtlinien** aus, und wählen Sie das Symbol aus, um eine neue Richtlinie hinzuzufügen.
6. Weisen Sie der Aufbewahrungsrichtlinie einen Namen zu, klicken Und scrollen Sie, um das soeben erstellte Aufbewahrungstag zu suchen und hinzuzufügen. Klicken Sie auf **Speichern**.
7. Wenden Sie schließlich die Aufbewahrungsrichtlinie auf das Postfach des Benutzers an: Navigieren Sie noch im Exchange Admin Center zu **"****Recipientsmailboxes** > ". Wählen Sie alle Benutzer aus, auf die Sie die Richtlinie anwenden möchten, und klicken Sie dann auf **"Bearbeiten"** (das Stiftsymbol).
8. Klicken Sie im Dialogfeld auf **Postfachfeatures**. Wenden Sie unter **"Aufbewahrungsrichtlinie**" die Richtlinie an, die Sie gerade > **Speichern** erstellt haben.
9. Anweisungen zum Anwenden der Richtlinie auf alle Benutzer finden Sie unter [Anwenden einer Aufbewahrungsrichtlinie auf Postfächer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
