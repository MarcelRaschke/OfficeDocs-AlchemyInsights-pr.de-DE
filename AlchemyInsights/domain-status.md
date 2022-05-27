---
title: Domänenstatus – Keine Dienste ausgewählt
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: d18451e03d0394329667b26d6659c220a5932b9b
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65709446"
---
# <a name="domain-status---no-services-selected"></a>Domänenstatus – Keine Dienste ausgewählt

**Keine Dienste ausgewählt** bedeutet, dass Sie keine Microsoft 365 Dienste wie Exchange Online, Skype for Business oder Intune und mobile Geräteverwaltung ausgewählt haben, die Microsoft 365 mit Ihren benutzerdefinierten Diensten verwenden können. Domäne. Wenn Sie Exchange Hybrid (Exchange lokal mit Exchange Online) oder externe Spamfilterung mit Exchange und keinem anderen Microsoft-Dienste verwenden, können Sie diese Nachricht ignorieren. Der Domänenintegritätsstatus ist nur für Domänen verfügbar, die direkt mit dem Dienst verbunden sind.

So wählen Sie Dienste für Ihre Domäne aus:

1. Aktivieren Sie **in Einstellungen** >  [**Domänen**](https://admin.microsoft.com/Adminportal/Home) das Kontrollkästchen neben der Domäne, wobei die Statusmeldung **"Keine Dienste" ausgewählt ist**.
1. Wählen Sie **"DNS verwalten** " aus, um den Domäneneinrichtungs-Assistenten zu starten.
    - Wenn Sie **"Eigene DNS-Einträge hinzufügen"** auswählen, achten Sie darauf, einen Dienst auszuwählen, wenn Sie dazu aufgefordert werden. Weitere Dienste könnten unter **"Erweiterte Optionen"** verfügbar sein.
    - Wenn Sie "**Zulassen, dass Microsoft Ihre DNS-Einträge hinzufügen**" oder "**Weitere Optionen** >  einrichten" auswählt, werden **Onlinedienste alle** verfügbaren Dienste für mich vorgeschlagen und automatisch ausgewählt.
1. Fahren Sie mit dem Assistenten fort, um das DNS-Setup und Ihre Dienstoptionen abzuschließen.
 
Weitere Hilfe zum Einrichten Ihrer Domäne finden Sie unter ["Hinzufügen von DNS-Einträgen zum Verbinden Ihrer Domäne"](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

