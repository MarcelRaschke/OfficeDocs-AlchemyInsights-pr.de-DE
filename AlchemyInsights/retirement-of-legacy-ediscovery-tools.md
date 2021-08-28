---
title: Einstellung von Legacy-eDiscovery-Tools
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074673"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Einstellung von Legacy-eDiscovery-Tools

Aufgrund der neuen und verbesserten eDiscovery-Funktionen im Microsoft 365 Compliance Center werden die folgenden eDiscovery-Tools und -Commandlets der Vorversion in den kommenden Monaten eingestellt:

- [In-Situ-eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) und [In-Situ-Speicher](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) im Exchange Admin Center.

- Die Exchange Online PowerShell-Cmdlets, die In-Place eDiscovery- und In-Place-Haltebereiche unterstützen. (Diese Cmdlets werden gemeinsam als *-MailboxSearch-Cmdlets identifiziert.) Dazu gehören die folgenden Cmdlets:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Das Cmdlet ["Search-Mailbox"](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) in Exchange Online PowerShell.
- Die folgenden Vorgänge in der Exchange-Webdienst-API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Zeitachse für die Einstellung:**
- **1. Juli 2020** Sie können keine neuen Suchvorgänge und Haltebereiche mehr erstellen, sondern vorhandene Suchen auf eigenes Risiko ausführen, bearbeiten und löschen. Der Microsoft-Support unterstützt In-Place eDiscovery-&-Haltebereiche im EAC nicht mehr.
    
- **Am 1. Oktober 2020** wird In-Place eDiscovery & Haltebereichsfunktionen im EAC im schreibgeschützten Modus platziert, sodass Sie nur vorhandene Suchvorgänge und Haltebereiche entfernen können.

**Weitere Informationen finden Sie unter:**

 - [Migrieren von eDiscovery-Legacysuchen und -haltebereichen zum Microsoft 365 Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Einstellung älterer eDiscovery-Tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Häufig gestellte Fragen zu In-Place eDiscovery und In-Place-Haltebereichen](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



