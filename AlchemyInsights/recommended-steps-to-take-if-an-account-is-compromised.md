---
title: Empfohlene Maßnahmen bei einem kompromittierten Konto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: 18cd624d36584be1f157dd6c039d14f3ffaf839f
ms.sourcegitcommit: 7d6400bbde052481a61de6a8e4067ce1f1b1e247
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/06/2021
ms.locfileid: "60800010"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a>Empfohlene Maßnahmen bei einem kompromittierten Konto

[VIDEO: Fixing a compromised account (Reparieren eines kompromittierten Kontos)](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. [Setzen Sie das Kennwort des Benutzers sofort zurück.](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) Übermitteln Sie das neue Kennwort nicht per E-Mail an den Endbenutzer.

2. Entfernen Sie alle auf Postfachebene festgelegten verdächtigen [Weiterleitungsadressen](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

3. Entfernen Sie alle innerhalb des Postfachs festgelegten verdächtigen [Posteingangsregeln](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED).

4. Navigieren Sie zum Microsoft 365 Defender-Portal unter <https://security.microsoft.com> \> **E-Mail und Zusammenarbeit** \> **Überprüfen** \> **Eingeschränkte Benutzer** oder direkt unter <https://security.microsoft.com/restrictedusers>. Wenn sich der Benutzer in der Liste befindet, wählen Sie ihn aus, und klicken Sie dann auf **Blockierung aufheben**. Führen Sie die Schritte im Flyoutbereich aus, und wählen Sie dann **Ja** aus, um die Aktion zu bestätigen. Das Konto sollte die Nachrichten in der Regel innerhalb einer Stunde erneut senden können.

5. Entfernen Sie das Benutzerkonto aus allen [administrative Rollengruppen](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles), bis Sie sicher sind, dass das Konto nicht mehr gefährdet ist.

Um das Risiko einer Datenschutzverletzung oder eines kompromittierten Kontos zukünftig zu minimieren, sollten Sie sich die [Microsoft 365 Security-Roadmap](https://docs.microsoft.com//office365/securitycompliance/security-roadmap) anschauen.
  