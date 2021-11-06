---
title: Identifizieren der externen E-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 5e99bd20c152df1caf95e721f30a47a45f5da031
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60799794"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ermitteln, wann die externe E-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Microsoft 365 Benutzer die externe E-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des Cmdlets **"Set-Mailbox"** überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokollsuche anzeigen. Hier erfahren Sie, wie Sie dies tun.

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - Überprüfen Sie, ob das Feld **"Aktivitäten"** **die Ergebnisse für alle Aktivitäten** enthält.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf **Ergebnisse filtern**, und geben Sie **Set-Mailbox** in das Aktivitätsfilterfeld ein.

5. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im angezeigten Detail-Flyout müssen Sie sich die Details der einzelnen Überwachungsdateneinträge ansehen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt.
   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter:** _ForwardingSmtpAddress_ gibt die E-Mail-Zieladresse an.
   - **UserId**: Der Benutzer, der die E-Mail-Weiterleitung für das Postfach im **Feld ObjectId** konfiguriert hat.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet hat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
