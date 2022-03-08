---
title: 'Fehler: Die Regeln auf diesem Computer stimmen nicht überein'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: a9493b0b9b6fb7008bff2dc88636d5ef1b01cbf5
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63083746"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fehler: Die Regeln auf diesem Computer stimmen nicht überein

Informationen zum aktualisierten Status dieses bekannten Problems finden Sie unter ["Die Regeln auf diesem Computer entsprechen nicht den Regeln in Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Das Outlook Team hat einen Fix in Build 12928.10000 implementiert. Der Fix ist bereits bei Insider Fast und wird Ende Juni 2020 zum monatlichen Kanal geleitet. Sobald Sie den festen Build haben, erhalten Sie möglicherweise ein letztes Mal die Eingabeaufforderung "Welche Regeln möchten Sie beibehalten". Wählen Sie "Server" aus, wenn Sie dazu aufgefordert werden, und wechseln Sie dann zurück zu Outlook und aktivieren Sie alle deaktivierten Regeln erneut.

Verwenden Sie die folgende Problemumgehung, bis die Korrektur verfügbar ist:

**Problemumgehung**: In aktuellen Berichten ist das Problem für diejenigen aufgetreten, die nur Clientregeln in Outlook Desktop erstellt haben. Wenn das Problem weiterhin auftritt, sollten Sie die Regeln löschen und dann Regeln nur in OWA (Outlook Web App) erstellen und bearbeiten, bis das Problem behoben ist.

Wenn Sie die Regeln nicht manuell löschen können, können Sie einen Outlook Befehl ausführen, wenn Sie Outlook starten, indem Sie Outlook.exe /cleanrules ausführen. Dadurch werden sowohl die Client- als auch die Serverregeln gelöscht. Sie löscht alle Regeln für alle Konten im Outlook Profil. Dieser Befehl wird im Artikel "Befehlszeilenoptionen" weiter dokumentiert.

