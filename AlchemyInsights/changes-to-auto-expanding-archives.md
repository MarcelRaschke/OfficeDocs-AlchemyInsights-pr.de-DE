---
title: Änderungen an Automatisch erweiternden Archiven
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 10/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "14097"
- "3100006"
ms.openlocfilehash: 00de6ecacc641a1595f319aa35842871c8431ddd
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62723625"
---
# <a name="changes-to-auto-expanding-archives"></a>Änderungen an Automatisch erweiternden Archiven

Wie im Beitrag des Nachrichtencenters „MC288051: (Aktualisiert) Anstehende Änderungen am automatisch erweiternden Archiv“ erwähnt, haben wir die Dokumentation zum automatisch erweiternden Archiv aktualisiert und den Grenzwert von 1,5 TB für Archivpostfächer festgelegt. 

Hier finden Sie weitere Informationen und Tipps:

- So überprüfen Sie die Gesamtgröße der Archive/Hilfsarchive:
    1. Herstellen einer Verbindung mit [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    1. Führen Sie das folgende Cmdlet aus: Get-MailboxStatistics -Archive |fl displayname,totalitemsize:

- Benutzer müssen möglicherweise Speicherplatz freimachen, indem sie Inhalte aus dem Archiv löschen. Wenden Sie sich an Ihren Complianceadministrator, um die spezifischen Anforderungen für Ihre Organisation zu ermitteln.

- Der Grenzwert von 1,5 TB kann nicht konfiguriert werden. Der Grenzwert gilt für alle SKUs/Lizenzen mit Archiven. 

- Wenn das Archiv voll ist oder es das Speicherkontingent erreicht, erhält der Benutzer eine Meldung wie die folgende: "Ihr Archivpostfach ist fast voll" oder "Ihr Archivpostfach ist voll".

Weitere Informationen zum Archivierungsfeature finden Sie unter [Übersicht zur automatische erweiternden Archivierung ](https://docs.microsoft.com/microsoft-365/compliance/autoexpanding-archiving)

Informationen zum Abrufen von Informationen zu den Ordnern in einem angegebenen Postfach finden Sie unter [Get-MailboxFolderStatistics](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderstatistics?view=exchange-ps&preserve-view=true).
