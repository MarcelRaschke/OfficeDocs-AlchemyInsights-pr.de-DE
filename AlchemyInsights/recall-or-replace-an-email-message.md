---
title: Zurückrufen oder Ersetzen einer E-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000260"
- "1860"
ms.date: 04/21/2020
ms.openlocfilehash: 4776af2465471ff4fd87b8be67a161f38b75a8ec
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66399963"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Zurückrufen oder Ersetzen einer E-Mail-Nachricht in Microsoft 365

- Sie können **nur Nachrichten zurückrufen, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine Gmail-Adresse gesendet wurde, können Sie sie nicht zurückrufen.
- Sie können **nur Nachrichten zurückrufen, die von Outlook für den PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Web sendet, können Sie sie nicht zurückrufen.
- Als Mandantenadministrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell zurückrufen** (Weitere Informationen finden Sie unter: [Suchen nach und Löschen von E-Mail-Nachrichten](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Sie können keine Nachrichten aus dem Admin Center zurückrufen. Scrollen Sie nach unten zu "Suchen und Löschen von E-Mail-Nachrichten in Ihrer Organisation", um weitere Informationen zu erhalten.

**Zurückrufen oder Ersetzen einer von Ihnen gesendeten E-Mail-Nachricht**

1. Wählen Sie im Ordnerbereich links im Outlook-Fenster den Ordner "Gesendete Elemente" aus.
2. Öffnen Sie die Nachricht, die Sie zurückrufen möchten. Sie müssen doppelklicken, um die Nachricht zu öffnen. Wenn Sie die Nachricht so auswählen, dass sie im Lesebereich angezeigt wird, können Sie die Nachricht nicht zurückrufen.
3. Wählen Sie auf der Registerkarte "Nachricht" **die Option "Aktionen** > **" aus, um diese Nachricht zurückzurufen**.
4. Wählen Sie **"Ungelesene Kopien dieser Nachricht löschen** " oder **"Ungelesene Kopien löschen" aus, ersetzen Sie sie durch eine neue Nachricht**, und wählen Sie dann **"OK**" aus.
5. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie " **Senden**" aus.
6. Der Erfolg oder Fehler eines Nachrichtenrückrufs hängt von den Einstellungen der Empfänger in Outlook ab.

Weitere Informationen, einschließlich der Überprüfung des Rückrufs, finden Sie unter ["Rückruf" oder "Ersetzen einer von Ihnen gesendeten E-Mail-Nachricht](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)".

***Wenn Sie in Ihrer Organisation nach E-Mail-Nachrichten suchen und diese löschen*** möchten, ist es am einfachsten, wenn Sie ein globaler Administrator sind. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rollengruppe "eDiscovery-Manager" oder der Verwaltungsrolle "Compliancesuche" hinzugefügt werden. Zum Löschen von Nachrichten müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Verwaltungsrolle "Suchen und Löschen" beitreten. Berechtigungen für diese Rollen werden im [Security & Compliance Center](https://protection.office.com/) zugewiesen.

1. [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu finden.
2. [Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Wenn Sie MFA (mehrstufige Authentifizierung) verwenden, lesen Sie ["Herstellen einer Verbindung mit Microsoft 365 Security & Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)".
