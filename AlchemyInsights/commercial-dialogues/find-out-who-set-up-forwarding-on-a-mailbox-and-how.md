---
title: Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: e8703b0af20e985395b8481912c5fa809e4bf8db
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62705769"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie

Wenn die externe Weiterleitung für ein Postfach festgelegt wurde, wird die Aktivität als Teil des **Cmdlets "Set-Mailbox"** überwacht. So finden Sie die Aktivität im Überwachungsprotokoll:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

   **Hinweis**: Wenn ein Hinweis angezeigt wird, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Select the date/time range in the **Start** and **End** boxes.
   - Überprüfen Sie, ob das Feld **"Aktivitäten** " **die Ergebnisse für alle Aktivitäten** enthält.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf die Spalte **"Aktivität** ", um die Ergebnisse zu sortieren, und suchen Sie nach **"Set-Mailbox"-** Einträgen.

5. Wählen Sie eine Aktivität in den Ergebnissen aus, um das Detail-Flyout zu öffnen. Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt:
   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter**: _ForwardingSmtpAddress_ gibt die E-Mail-Zieladresse an.
   - **UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox) hat.
