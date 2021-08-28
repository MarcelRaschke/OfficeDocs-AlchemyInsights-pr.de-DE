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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317807"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie

Wenn die externe Weiterleitung für ein Postfach festgelegt wurde, wird die Aktivität als Teil des **Cmdlets "Set-Mailbox"** überwacht. So finden Sie die Aktivität im Überwachungsprotokoll:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> zu **"Lösungsüberwachung".** \>  Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://compliance.microsoft.com/auditlogsearch> wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **"Überwachen".** Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://security.microsoft.com/auditlogsearch> wechseln.

   **Hinweis:** Wenn Eine Benachrichtigung angezeigt wird, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.

2. Überprüfen Sie auf der Seite **"Überwachung",** ob die Registerkarte **"Suchen"** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - Überprüfen Sie, ob das Feld **"Aktivitäten"** **die Ergebnisse für alle Aktivitäten** enthält.

3. Wenn Sie fertig sind, klicken Sie auf **Suchen.** Die Aktivitäten werden auf der neuen **Überwachungssuchseite** angezeigt.

4. Klicken Sie in den Ergebnissen auf die Spalte **"Aktivität",** um die Ergebnisse zu sortieren, und suchen Sie nach **"Set-Mailbox"-Einträgen.**

5. Wählen Sie eine Aktivität in den Ergebnissen aus, um das Detail-Flyout zu öffnen. Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der E-Mail-Weiterleitung zusammenhängt:
   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter:** _ForwardingSmtpAddress_ gibt die E-Mail-Zieladresse an.
   - **UserId**: Der Benutzer, der die E-Mail-Weiterleitung für das Postfach im **Feld ObjectId** konfiguriert hat.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet hat.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
