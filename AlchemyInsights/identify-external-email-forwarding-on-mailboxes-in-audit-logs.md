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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331158"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ermitteln, wann die externe E-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Microsoft 365 Benutzer die externe E-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des Cmdlets **"Set-Mailbox"** überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokollsuche anzeigen. Hier erfahren Sie, wie Sie dies tun.

1. Führen Sie einen der folgenden Schritte aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **"Lösungsüberwachung".** \>  Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://compliance.microsoft.com/auditlogsearch> wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **"Überwachen".** Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://sip.security.microsoft.com/auditlogsearch> wechseln.

2. Überprüfen Sie auf der Seite **"Überwachung",** ob die Registerkarte **"Suchen"** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - Überprüfen Sie, ob das Feld **"Aktivitäten"** **die Ergebnisse für alle Aktivitäten** enthält.

3. Wenn Sie fertig sind, klicken Sie auf **Suchen.** Die Aktivitäten werden auf der neuen **Überwachungssuchseite** angezeigt.

4. Klicken Sie in den Ergebnissen auf **"Ergebnisse filtern",** und geben **Sie "Set-Mailbox"** im Aktivitätsfilterfeld ein.

5. Wählen Sie einen Überwachungsdatensatz in den Ergebnissen aus. Klicken Sie im **Flyout "Details"** auf **"Weitere Informationen".** Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt.

   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter:** _ForwardingSmtpAddress_ gibt die E-Mail-Zieladresse an.
   - **UserId**: Der Benutzer, der die E-Mail-Weiterleitung für das Postfach im **Feld ObjectId** konfiguriert hat.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet hat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
