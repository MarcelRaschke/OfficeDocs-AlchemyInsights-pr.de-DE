---
title: Zurückrufen oder Ersetzen einer E-Mail-Nachricht durch Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 9000260
ms.date: 04/21/2020
ms.openlocfilehash: c02da2bcefa0be30aaae439c7b5b595d422e808d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66303670"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Zurückrufen oder Ersetzen einer Outlook-E-Mail-Nachricht

- Als Administrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell zurückrufen**. Sie können keine Nachrichten aus dem Admin Center zurückrufen.
- Sie können **nur Nachrichten zurückrufen, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine Gmail-Adresse gesendet wurde, können Sie sie nicht zurückrufen.
- Sie können **nur Nachrichten zurückrufen, die von Outlook 2016 auf dem PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Web sendet, können Sie sie nicht zurückrufen.

So rufen Sie eine E-Mail-Nachricht zurück oder ersetzen sie:

1. Wählen Sie im Ordnerbereich links im Outlook-Fenster den Ordner "Gesendete Elemente" aus.
1. Doppelklicken Sie auf die Nachricht, die Sie zurückrufen möchten, um sie zu öffnen.
1. Wählen Sie die Registerkarte **"Nachricht** " und dann " **Aktionen** > **" aus, um diese Nachricht zurückzurufen**.
1. Wählen Sie **"Ungelesene Kopien dieser Nachricht löschen** " oder " **Ungelesene Kopien löschen" aus, ersetzen Sie sie durch eine neue Nachricht**, und wählen Sie dann **"OK**" aus.
1. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie " **Senden**" aus.
1. Der Erfolg oder Fehler eines Nachrichtenrückrufs hängt von den Einstellungen des Empfängers in Outlook ab. Schritte zum Überprüfen des Rückrufs finden Sie [in diesem Artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation

- Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rolle "eDiscovery-Manager" oder der Verwaltungsrolle "Compliancesuche" hinzugefügt werden, um nach Nachrichten zu suchen. Zum Löschen von Nachrichten müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Verwaltungsrolle "Suchen und Löschen" beitreten. Berechtigungen für diese Rollen werden im [Security and Compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731) zugewiesen.
- [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu finden.
- [Stellen Sie eine Verbindung mit Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps&preserve-view=true) her.

Wenn Sie die mehrstufige Authentifizierung verwenden, lesen Sie ["Herstellen einer Verbindung mit Microsoft 365 Security and Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps&preserve-view=true)".
