---
title: Behandeln falsch positiver oder negativer Spam- oder Phishingnachrichten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: ''
ms.openlocfilehash: 233b3c712d4f55f42b469c26b3bb332c80177506
ms.sourcegitcommit: 29a90a6b7a52ec8599daffabf6089f1e0d72e2aa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/20/2022
ms.locfileid: "66912422"
---
# <a name="handle-false-positive-or-negative-spam-or-phishing-messages"></a>Behandeln falsch positiver oder negativer Spam- oder Phishingnachrichten

**Gute Nachrichten werden im Junk-Ordner oder in Quarantäne als Spam oder Phishing gekennzeichnet**

- [Senden Sie Nachrichten mit Microsoft 365 Defender](https://go.microsoft.com/fwlink/?linkid=2167511) zur Analyse aller sich auswirkenden Richtlinien und Regeln. Select **Should not been blocked** when prompted to allow similar messages. Die Ergebnisse sind im Flyout "Übermittlungsdetails" verfügbar.
- Damit Ziel-E-Mail-Systeme ihren Nachrichten vertrauen können, sollten Absender Nachrichten an [SPF](https://go.microsoft.com/fwlink/?linkid=2169980), [DKIM](https://go.microsoft.com/fwlink/?linkid=2097807) und [DMARC](https://go.microsoft.com/fwlink/?linkid=2170079) ausrichten.
- Ausführliche Informationen finden Sie in der schrittweisen Anleitung [zum Umgang mit legitimen E-Mails, die mithilfe von Microsoft Defender for Office 365 blockiert werden (falsch positiv](https://docs.microsoft.com/microsoft-365/security/office-365-security/step-by-step-guides/how-to-handle-false-positives-in-microsoft-defender-for-office-365)).

**Ungültige Nachrichten wie Spam-, Phishing- oder Schadsoftwarenachrichten im Posteingang**

- Zur Analyse [senden Sie Nachrichten mit Microsoft 365 Defender](https://go.microsoft.com/fwlink/?linkid=2167511). Select **Should have been blocked** when prompted to block similar messages. Die Ergebnisse sind im Flyout "Übermittlungsdetails" verfügbar.
- Ausführliche Informationen finden Sie in der schrittweisen Anleitung [zum Umgang mit schädlichen E-Mails, die an Empfänger (Falsch negative Werte) übermittelt werden, mithilfe von Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/step-by-step-guides/how-to-handle-false-negatives-in-microsoft-defender-for-office-365).
- Weitere Informationen zu Übermittlungen finden Sie in [den Microsoft-Dokumenten](https://go.microsoft.com/fwlink/?linkid=2170621) oder im Video [Microsoft 365 Defender Unified-Übermittlungen](https://www.microsoft.com/videoplayer/embed/RE50HhM).

**Zusätzliche Empfehlungen**

- Microsoft Defender for Office 365 Plan 2- und E5-Kunden können Beispiele direkt aus dem [Explorer](https://go.microsoft.com/fwlink/?linkid=2201239) übermitteln.
- Verwalten Sie Ihre Filterüberschreibungen sicher in der [Mandanten-Zulassungs-/Sperrliste](https://go.microsoft.com/fwlink/?linkid=2166981). Das Hinzufügen dauerhafter Außerkraftsetzungen wird nicht empfohlen. Weitere Informationen finden Sie unter ["Warnungen vor der Umgehung Office 365 Spamfiltern"](https://docs.microsoft.com/exchange/troubleshoot/antispam-and-protection/cautions-against-bypassing-spam-filters).
- Ermöglichen Sie Endbenutzern, Nachrichten an Microsoft zu melden, um die Effektivität von E-Mail-Schutztechnologien zu verbessern. Weitere Informationen finden [Sie unter Aktivieren der Berichtsnachricht oder der Berichtsphishing-Add-Ins](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in).
- Befolgen Sie die [Microsoft-Sicherheitsbewertungsempfehlungen](https://go.microsoft.com/fwlink/?linkid=2167634) , um Ihre Organisation vor Bedrohungen zu schützen und die Sicherheit zu verbessern.

Weitere Informationen finden Sie unter [Verwalten der Zulassungs-/Sperrliste für Mandanten](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list), [Antispam-Nachrichtenkopfzeilen in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers) und [des Ausgehenden Spamschutzes in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls).

Wenn Sie mit Exchange Online Protection und Microsoft Defender for Office 365 noch nicht fertig sind, lesen Sie die Setuphandbücher für [EOP](https://admin.microsoft.com/AdminPortal/Home#/modernonboarding/setupexchangeonlineprotection) und [MDO](https://go.microsoft.com/fwlink/?linkid=2190925).