---
title: Änderungen an Automatisch erweiternden Archiven
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "3100006"
- "14097"
ms.date: 10/14/2021
ms.openlocfilehash: 9d225b5b016302f8654e4b71a0a92855e24c93cf
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66370047"
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
