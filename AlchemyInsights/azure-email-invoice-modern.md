---
title: Moderne Azure-E-Mail-Rechnungsstellung
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082833"
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
