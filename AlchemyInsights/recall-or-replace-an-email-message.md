---
title: Rückruf oder Ersetzen einer E-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: ecdbf5426a6fe274320036370a00059d9523d8a1
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63200563"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Rückruf oder Ersetzen einer E-Mail-Nachricht in Microsoft 365

- Sie können **sich nur an Nachrichten erinnern, die an Personen in Ihrer Organisation gesendet werden**. Wenn die Nachricht beispielsweise an eine Gmail-Adresse gesendet wurde, können Sie sie nicht mehr merken.
- Sie können **nur Nachrichten zurückrufen, die von Outlook für den PC gesendet wurden**. Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Web sendet, können Sie sie nicht mehr merken.
- Als Mandantenadministrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell abrufen** (Weitere Informationen finden Sie unter: [Suchen nach und Löschen von E-Mail-Nachrichten](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Sie können keine Nachrichten aus dem Admin Center abrufen. Scrollen Sie nach unten zu "Suchen und Löschen von E-Mail-Nachrichten in Ihrer Organisation", um weitere Informationen zu erhalten.

**Rückrufen oder Ersetzen einer E-Mail-Nachricht, die Sie gesendet haben**

1. Wählen Sie im Ordnerbereich auf der linken Seite des fensters Outlook den Ordner "Gesendete Elemente" aus.
2. Öffnen Sie die Nachricht, die Sie sich merken möchten. Sie müssen doppelklicken, um die Nachricht zu öffnen. Wenn Sie die Nachricht so auswählen, dass sie im Lesebereich angezeigt wird, können Sie die Nachricht nicht zurückrufen.
3. From the Message tab, select **Actions** > **Recall This Message**.
4. Wählen Sie **"Ungelesene Kopien dieser Nachricht löschen** " oder " **Ungelesene Kopien löschen" aus, und ersetzen Sie sie durch eine neue Nachricht**, und wählen Sie dann **"OK**" aus.
5. Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **"Senden**" aus.
6. Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen der Empfänger in Outlook ab.

Weitere Informationen, einschließlich der Überprüfung des Rückrufs, finden Sie unter [Rückruf oder Ersetzen einer E-Mail-Nachricht, die Sie gesendet haben](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Um E-Mail-Nachrichten in Ihrer Organisation zu suchen und zu löschen***, ist es am einfachsten, wenn Sie ein globaler Administrator sind. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rollengruppe "eDiscovery-Manager" oder der Verwaltungsrolle "Compliancesuche" hinzugefügt werden. Um Nachrichten zu löschen, müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Verwaltungsrolle "Suchen und Löschen" beitreten. Berechtigungen für diese Rollen werden im [Security & Compliance Center](https://protection.office.com/) zugewiesen.

1. [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu finden.
2. [Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Wenn Sie MFA (mehrstufige Authentifizierung) verwenden, lesen Sie [Verbinden zum Microsoft 365 Security & Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
