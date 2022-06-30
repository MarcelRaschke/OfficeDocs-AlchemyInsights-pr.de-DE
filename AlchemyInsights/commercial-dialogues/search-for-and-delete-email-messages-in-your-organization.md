---
title: Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: 735a5222ebfc13a072f066cf2642d2631df8f482
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66379677"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation

Führen Sie die folgenden Schritte aus:

1. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der **Rollengruppe "eDiscovery-Manager** " oder der **Verwaltungsrolle "Compliancesuche**" hinzugefügt werden, um nach Nachrichten zu suchen. Zum Löschen von Nachrichten müssen Sie der **Rollengruppe "Organisationsverwaltung** " oder der **Verwaltungsrolle "Suchen und Löschen**" beitreten. Berechtigungen für diese Rollen werden im [Security & Compliance Center zugewiesen.](https://protection.office.com)
2. [Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/office365/securitycompliance/content-search) , um die zu löschende Nachricht zu finden.
3. [Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Wenn Sie MFA verwenden, lesen Sie die folgenden Anweisungen: [Herstellen einer Verbindung mit Security & Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Löschen Sie die Nachricht: Führen Sie das `New-ComplianceSearchAction` Cmdlet aus, um die Nachricht zu löschen. Gelöschte Nachrichten werden in den Ordner „Wiederherstellbare Elemente“ des Benutzers verschoben. Ein Beispielbefehl finden Sie unter [Schritt 3: Löschen der Nachricht.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
