---
title: 1336 RecoverableItems-Ordner ist voll
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061755"
---
# <a name="the-recoverable-items-folder-is-full"></a>Der Ordner "Wiederherstellbare Elemente" ist voll.

Bei Exchange Online Postfächern beträgt der Standardmäßige Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" 30 GB. Der Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" wird automatisch auf 100 GB erhöht, wenn das Postfach in das Beweissicherungsverfahren, eDiscovery-Archiv oder einer Aufbewahrungsrichtlinie versetzt wird.

Wenn der Ordner "Wiederherstellbare Elemente" das Speicherlimit erreicht, wird die Postfachfunktionalität wie folgt beeinträchtigt:

- Der Benutzer kann keine Elemente aus dem Postfach löschen.

- Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.

- Bei Postfächern, für die die Wiederherstellung einzelner Elemente aktiviert ist oder die in den Haltebereich versetzt werden, kann der Kopie-bei-Schreib-Seitenschutz keine Versionen der vom Benutzer bearbeiteten Elemente verwalten.

- Für Postfächer, für die die Postfachüberwachungsprotokollierung aktiviert ist, können keine Postfachüberwachungsprotokolleinträge im Unterordner "Überwachungen" im Ordner "Wiederherstellbare Elemente" gespeichert werden.

Für Postfächer, die nicht in der Warteschleife sind, können Administratoren den `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Befehl in Exchange Online PowerShell verwenden, um Elemente im Ordner "Wiederherstellbare Elemente" zu löschen. Weitere Informationen finden Sie in den folgenden Themen:

- [Suchen nach und Löschen von Nachrichten](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Für Postfächer, die in der Warteschleife sind, müssen Administratoren den Haltebereich entfernen, bevor sie Elemente aus dem Ordner "Wiederherstellbare Elemente" löschen können. Weitere Informationen finden Sie unter [Löschen von Elementen im Ordner "Wiederherstellbare Elemente" von cloudbasierten Postfächern im Haltebereich.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Um zu verhindern, dass der Ordner "Wiederherstellbare Elemente" vollständig wird, können Administratoren das Speicherlimit des Ordners "Wiederherstellbare Elemente" für Postfächer erhöhen, die in der Warteschleife sind, und eine Postfachaufbewahrungsrichtlinie einrichten, die Elemente aus dem Ordner "Wiederherstellbare Elemente" in das Archivpostfach des Benutzers verschiebt. Siehe [Erhöhen des Kontingents für wiederherstellbare Elemente für Postfächer im Haltebereich.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
