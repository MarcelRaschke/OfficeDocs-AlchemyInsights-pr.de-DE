---
title: Empfohlene Maßnahmen bei einem kompromittierten Konto
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: 27b68c2c67db7d8c0dfbccfde654d0dc0934f36a
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61981426"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a>Empfohlene Maßnahmen bei einem kompromittierten Konto

[VIDEO: Fixing a compromised account (Reparieren eines kompromittierten Kontos)](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. [Setzen Sie das Kennwort des Benutzers sofort zurück.](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) Übermitteln Sie das neue Kennwort nicht per E-Mail an den Endbenutzer.

2. Entfernen Sie alle auf Postfachebene festgelegten verdächtigen [Weiterleitungsadressen](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

3. Entfernen Sie alle innerhalb des Postfachs festgelegten verdächtigen [Posteingangsregeln](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED).

4. Navigieren Sie zum Microsoft 365 Defender-Portal unter <https://security.microsoft.com> \> **E-Mail und Zusammenarbeit** \> **Überprüfen** \> **Eingeschränkte Benutzer** oder direkt unter <https://security.microsoft.com/restrictedusers>. Wenn sich der Benutzer in der Liste befindet, wählen Sie ihn aus, und klicken Sie dann auf **Blockierung aufheben**. Führen Sie die Schritte im Flyoutbereich aus, und wählen Sie dann **Ja** aus, um die Aktion zu bestätigen. Das Konto sollte die Nachrichten in der Regel innerhalb einer Stunde erneut senden können.

5. Entfernen Sie das Benutzerkonto aus allen [administrative Rollengruppen](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles), bis Sie sicher sind, dass das Konto nicht mehr gefährdet ist.

Um das Risiko einer Datenschutzverletzung oder eines kompromittierten Kontos zukünftig zu minimieren, sollten Sie sich die [Microsoft 365 Security-Roadmap](https://docs.microsoft.com//office365/securitycompliance/security-roadmap) anschauen.
  