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
ms.localizationpriority: medium
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 86d0e0725fd8c34ef25ed28049e57fd191410c9d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63275597"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ermitteln, wann die externe E-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Microsoft 365 Benutzer die externe E-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des **Cmdlets "Set-Mailbox**" überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokollsuche anzeigen. Hier erfahren Sie, wie Sie dies tun.

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Select the date/time range in the **Start** and **End** boxes.
   - Überprüfen Sie, ob das Feld **"Aktivitäten** " **die Ergebnisse für alle Aktivitäten** enthält.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf **Ergebnisse filtern**, und geben Sie **Set-Mailbox** in das Aktivitätsfilterfeld ein.

5. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im angezeigten Detail-Flyout müssen Sie sich die Details der einzelnen Überwachungsdateneinträge ansehen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt.
   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter**: _ForwardingSmtpAddress_ gibt die E-Mail-Zieladresse an.
   - **UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox) hat.
