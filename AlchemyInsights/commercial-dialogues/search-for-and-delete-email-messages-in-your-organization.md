---
title: Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948882"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation

Führen Sie die folgenden Schritte aus:

1. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der **Rollengruppe "eDiscovery-Manager"** oder der **Verwaltungsrolle "Compliancesuche"** hinzugefügt werden, um nach Nachrichten zu suchen. Um Nachrichten zu löschen, müssen Sie der **Rollengruppe "Organisationsverwaltung"** oder der **Verwaltungsrolle "Suchen und Löschen"** beitreten. Berechtigungen für diese Rollen werden im [Security & Compliance Center zugewiesen.](https://protection.office.com)
2. [Erstellen Sie eine Inhaltssuche,](https://docs.microsoft.com/office365/securitycompliance/content-search) um die zu löschende Nachricht zu finden.
3. [Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Wenn Sie MFA verwenden, lesen Sie die folgenden Anweisungen: [Verbinden zu Security & Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Löschen Sie die Nachricht: Führen Sie das `New-ComplianceSearchAction` Cmdlet aus, um die Nachricht zu löschen. Gelöschte Nachrichten werden in den Ordner "Wiederherstellbare Elemente" eines Benutzers verschoben. Einen Beispielbefehl finden Sie unter [Schritt 3: Löschen der Nachricht.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
