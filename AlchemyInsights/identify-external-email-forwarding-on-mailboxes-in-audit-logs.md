---
title: Identifizieren der externen E-Mail-Weiterleitung in Postfächern in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100005"
- "1369"
ms.date: 04/21/2020
ms.openlocfilehash: 71ea049128c75132cb17e45f39e93663d3c69983
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66405796"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifizieren, wann die externe E-Mail-Weiterleitung für Postfächer konfiguriert ist

Wenn ein Microsoft 365-Benutzer die externe E-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des Cmdlets **"Set-Mailbox"** überwacht. Sie können die Aktivität mithilfe der Überwachungsprotokollsuche anzeigen. Hier erfahren Sie, wie Sie dies tun.

1. Führen Sie einen der folgenden Schritte aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://sip.security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **"Start** " und " **Ende** " aus.
   - Überprüfen Sie, ob das Feld **"Aktivitäten** " **ergebnisse für alle Aktivitäten anzeigen** enthält.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf **Ergebnisse filtern**, und geben Sie **Set-Mailbox** in das Aktivitätsfilterfeld ein.

5. Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Im daraufhin angezeigten Detailflyout müssen Sie die Details jedes Überwachungsdatensatzes überprüfen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt.
   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-E-Mail-Adresse an.
   - **UserId**: Der Benutzer, der die E-Mail-Weiterleitung für das Postfach im Feld **"ObjectId** " konfiguriert hat.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox) hat.
