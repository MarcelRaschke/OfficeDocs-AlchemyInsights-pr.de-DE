---
title: Moderne Azure-E-Mail-Rechnungsstellung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 6f5d8423c4c9d6f04102f12a69a1b848bdc01ed1
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66329925"
---
# <a name="email-invoicing-in-azure"></a>E-Mail-Rechnungsstellung in Azure

Sie müssen über die Rolle "Besitzer" oder "Mitwirkender" für das Abrechnungsprofil oder das entsprechende Abrechnungskonto verfügen, um die Einstellungen für E-Mail-Rechnungen aktualisieren zu können. Nach der Aktivierung erhalten alle Benutzer mit der Rolle "Besitzer", "Mitwirkender", "Leser" und "Rechnungsadministrator" die Rechnung per E-Mail.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
2. Suchen Sie nach **Kostenverwaltung und Abrechnung**.
3. Wählen Sie auf der linken Seite **Rechnungen** und dann oben auf der Seite **E-Mail-Rechnung** aus.
4. Wenn Sie über mehrere Abrechnungsprofile verfügen, wählen Sie das gewünschte Abrechnungsprofil und dann **Aktivieren** aus.

5. Wählen Sie **Aktualisieren** aus.
6. Wenn Sie über mehrere Abrechnungsprofile verfügen, wählen Sie das gewünschte Abrechnungsprofil und dann **Aktivieren** aus.

Sie können anderen Personen das Anzeigen, Herunterladen und Begleichen von Rechnungen gestatten, indem Sie ihnen die Rolle "Rechnungsadministrator" für ein MCA- oder MPA-Abrechnungsprofil zuweisen. Wenn Sie den Erhalt von Rechnungen per E-Mail aktiviert haben, erhalten die Benutzer die Rechnungen ebenfalls per E-Mail.

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.
2. Suchen Sie nach **Kostenverwaltung und Abrechnung**.
3. Wählen Sie auf der linken Seite **Abrechnungsprofile** aus. Wählen Sie in der Liste der Abrechnungsprofile jenes aus, für das Sie jemandem die Rolle "Rechnungsadministrator" zuweisen möchten.
4. Wählen Sie auf der linken Seite **Zugriffssteuerung (IAM)** und dann oben auf der Seite **Hinzufügen** aus.

Wählen Sie in der Dropdownliste der Rollen **Rechnungsadministrator** aus. Geben Sie die E-Mail-Adresse des Benutzers ein, der Zugriff erhalten soll. Wählen Sie **Speichern** aus, damit die Rolle zugewiesen wird.
