---
title: Outlook Desktop-Rückruf oder Ersetzen einer E-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bc6a11a4cf924f98616d1aa89e202c6d1635c32e
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62566564"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Rückruf oder Ersetzen einer Outlook E-Mail-Nachricht

- Als Administrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell zurückrufen**. Sie können keine Nachrichten aus dem Admin Center abrufen.
- Sie können **sich nur an Nachrichten erinnern, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine Gmail-Adresse gesendet wurde, können Sie sie nicht mehr merken.
- Sie können **nur Nachrichten zurückrufen, die von Outlook 2016 auf dem PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Web sendet, können Sie sie nicht mehr merken.

So rufen Sie eine E-Mail-Nachricht zurück oder ersetzen sie:

1. Wählen Sie im Ordnerbereich auf der linken Seite des fensters Outlook den Ordner "Gesendete Elemente" aus.
1. Doppelklicken Sie auf die Nachricht, die Sie erneut aufrufen möchten, um sie zu öffnen.
1. Select the **Message** tab, and then select **Actions** > **Recall This Message**.
1. Wählen Sie **"Ungelesene Kopien dieser Nachricht löschen** " oder " **Ungelesene Kopien löschen" aus, ersetzen Sie sie durch eine neue Nachricht**, und wählen Sie dann **"OK**" aus.
1. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **"Senden**" aus.
1. Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen des Empfängers in Outlook ab. Schritte zum Überprüfen des Rückrufs finden Sie in [diesem Artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation

- Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rolle "eDiscovery-Manager" oder der Verwaltungsrolle "Compliancesuche" hinzugefügt werden, um nach Nachrichten zu suchen. Um Nachrichten zu löschen, müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Verwaltungsrolle "Suchen und Löschen" beitreten. Berechtigungen für diese Rollen werden im [Security and Compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731) zugewiesen.
- [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu finden.
- [Verbinden zu Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps&preserve-view=true).

Wenn Sie die mehrstufige Authentifizierung verwenden, lesen Sie [Verbinden zum Microsoft 365 Security and Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps&preserve-view=true).
