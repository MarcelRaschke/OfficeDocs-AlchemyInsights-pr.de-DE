---
title: 'Fehler: Die Regeln auf diesem Computer stimmen nicht überein'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1800021"
- "3518"
ms.openlocfilehash: 3b29a915150b80ecc1b51f042874e465844c243e
ms.sourcegitcommit: 28a0efb945a4827518e4b6a3a8c804d4ba2e3349
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/01/2022
ms.locfileid: "66595615"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fehler: Die Regeln auf diesem Computer stimmen nicht überein

Wenn Sie den aktualisierten Status dieses bekannten Problems anzeigen möchten, lesen Sie [die Regeln auf diesem Computer, die nicht mit den Regeln in Microsoft Exchange übereinstimmen](https://support.microsoft.com/office/the-rules-on-this-computer-do-not-match-the-rules-on-microsoft-exchange-d032e037-b224-429e-b325-633afde9b5f0).

Das Outlook-Team hat einen Fix in Build 12928.10000 implementiert. Der Fix ist bereits bei Insider Fast und wird Ende Juni 2020 zum monatlichen Kanal wechseln. Sobald Sie den festen Build haben, erhalten Sie möglicherweise ein letztes Mal die Eingabeaufforderung "Welche Regeln möchten Sie beibehalten". Wählen Sie "Server" aus, wenn Sie dazu aufgefordert werden, und wechseln Sie dann zurück in Outlook, und aktivieren Sie alle deaktivierten Regeln erneut.

Verwenden Sie die folgende Problemumgehung, bis der Fix verfügbar ist:

**Problemumgehung**: In den letzten Berichten ist das Problem für diejenigen aufgetreten, die nur Clientregeln in Outlook Desktop erstellt haben. Wenn das Problem weiterhin auftritt, sollten Sie die Regeln löschen und dann regeln nur in OWA (Outlook Web App) erstellen und bearbeiten, bis das Problem behoben ist.

Wenn Sie die Regeln nicht manuell löschen können, können Sie beim Starten von Outlook einen Outlook-Befehl ausführen, indem Sie Outlook.exe /cleanrules ausführen. Dadurch werden sowohl die Client- als auch die Serverregeln gelöscht. Alle Regeln für alle Konten im Outlook-Profil werden gelöscht. Dieser Befehl ist im Artikel "Befehlszeilenoptionen" weiter dokumentiert.

