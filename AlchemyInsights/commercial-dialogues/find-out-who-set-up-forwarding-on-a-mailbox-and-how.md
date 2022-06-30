---
title: Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100005"
- "7327"
ms.date: 02/26/2021
ms.openlocfilehash: 22316cdb6606e5e688fc5e605f883483e38a3821
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66414182"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie

Wenn die externe Weiterleitung für ein Postfach festgelegt wurde, wird die Aktivität als Teil des Cmdlets **"Set-Mailbox** " überwacht. Hier erfahren Sie, wie Sie die Aktivität im Überwachungsprotokoll finden:

1. Führen Sie eine der folgenden Aktionen aus:
   - Im Microsoft Purview-Complianceportal unter <https://compliance.microsoft.com> wechseln Sie zu **Lösungen** \> **Überwachung**. Oder verwenden Sie <https://compliance.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **Überwachung**. Oder verwenden Sie <https://security.microsoft.com/auditlogsearch>, um direkt zur Seite **Überwachung** zu wechseln.

   **Hinweis**: Wenn eine Benachrichtigung angezeigt wird, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus vorherigen Datumsangaben abrufen.

2. Vergewissern Sie sich, auf der Seite **Überwachung**, dass die Registerkarte **Suche** ausgewählt ist, und konfigurieren Sie dann die folgenden Einstellungen:
   - Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **"Start** " und " **Ende** " aus.
   - Überprüfen Sie, ob das Feld **"Aktivitäten** " **ergebnisse für alle Aktivitäten anzeigen** enthält.

3. Wenn Sie den Vorgang abgeschlossen haben, klicken Sie auf **Suchen**. Die Aktivitäten werden auf der neuen Seite **Suche überwachen** angezeigt.

4. Klicken Sie in den Ergebnissen auf die Spalte **"Aktivität** ", um die Ergebnisse zu sortieren, und suchen Sie nach **Set-Mailbox-Einträgen** .

5. Wählen Sie in den Ergebnissen eine Aktivität aus, um das Detail-Flyout zu öffnen. Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob sich die Aktivität auf die E-Mail-Weiterleitung bezieht:
   - **ObjectId**: Der Aliaswert des Postfachs, das geändert wurde.
   - **Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-E-Mail-Adresse an.
   - **UserId**: Der Benutzer, der die E-Mail-Weiterleitung für das Postfach im Feld **"ObjectId** " konfiguriert hat.

Weitere Informationen finden Sie unter [Ermitteln, wer die E-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox) hat.
