---
title: Domänenstatus – Keine Dienste ausgewählt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9006491"
- "11094"
ms.date: 04/30/2021
ms.openlocfilehash: ce066ff141854084c6308fe98e5bc4c97e13fe1e
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66518196"
---
# <a name="domain-status---no-services-selected"></a>Domänenstatus – Keine Dienste ausgewählt

**Keine Dienste ausgewählt** bedeutet, dass Sie keine Microsoft 365-Dienste wie Exchange Online, Skype for Business oder Intune und mobile Geräteverwaltung für Microsoft 365 ausgewählt haben, die mit Ihrer benutzerdefinierten Domäne verwendet werden sollen. Wenn Sie Exchange Hybrid (exchange lokal mit Exchange Online) oder externe Spamfilterung mit Exchange und keinen anderen Microsoft-Diensten verwenden, können Sie diese Nachricht ignorieren. Der Domänenintegritätsstatus ist nur für Domänen verfügbar, die direkt mit dem Dienst verbunden sind.

So wählen Sie Dienste für Ihre Domäne aus:

1. Aktivieren **Sie in den Einstellungsdomänen** >  das Kontrollkästchen neben der Domäne, wobei die Statusmeldung **"Keine Dienste" ausgewählt ist**.[](https://admin.microsoft.com/Adminportal/Home)
1. Wählen Sie **"DNS verwalten** " aus, um den Domäneneinrichtungs-Assistenten zu starten.
    - Wenn Sie **"Eigene DNS-Einträge hinzufügen"** auswählen, achten Sie darauf, einen Dienst auszuwählen, wenn Sie dazu aufgefordert werden. Weitere Dienste könnten unter **"Erweiterte Optionen"** verfügbar sein.
    - Wenn Sie "**Zulassen, dass Microsoft Ihre DNS-Einträge hinzufügen**" oder "**Weitere Optionen** >  einrichten" auswählt, werden **Onlinedienste alle** verfügbaren Dienste für mich vorgeschlagen und automatisch ausgewählt.
1. Fahren Sie mit dem Assistenten fort, um das DNS-Setup und Ihre Dienstoptionen abzuschließen.
 
Weitere Hilfe zum Einrichten Ihrer Domäne finden Sie unter ["Hinzufügen von DNS-Einträgen zum Verbinden Ihrer Domäne"](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

