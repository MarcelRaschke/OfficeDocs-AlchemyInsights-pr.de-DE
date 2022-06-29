---
title: 1336 Der Ordner "RecoverableItems" ist voll.
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3700003"
- "1336"
ms.date: 04/21/2020
ms.openlocfilehash: ffcd6a6ceb6c8d5d3067010edcfc0ef4216cf1dc
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66418738"
---
# <a name="the-recoverable-items-folder-is-full"></a>Der Ordner "Wiederherstellbare Elemente" ist voll.

Für Exchange Online Postfächer beträgt der Standardspeichergrenzwert für den Ordner "Wiederherstellbare Elemente" 30 GB. Der Speichergrenzwert für den Ordner "Wiederherstellbare Elemente" wird automatisch auf 100 GB erhöht, wenn das Postfach im Beweissicherungsverfahren, eDiscovery-Speicher oder einer Aufbewahrungsrichtlinie zugewiesen ist.

Wenn der Ordner "Wiederherstellbare Elemente" das Speicherlimit erreicht, ist die Postfachfunktionalität auf folgende Weise betroffen:

- Der Benutzer kann keine Elemente aus dem Postfach löschen.

- Der Assistent für verwaltete Ordner kann keine Elemente auf der Grundlage von Aufbewahrungstags oder Einstellungen für verwaltete Ordner löschen.

- Bei Postfächern, für die die Wiederherstellung einzelner Elemente aktiviert oder im Haltebereich platziert wurde, kann der Kopier-bei-Schreib-Seitenschutz keine Versionen von Elementen verwalten, die vom Benutzer bearbeitet wurden.

- Bei Postfächern, für die die Postfachüberwachungsprotokollierung aktiviert ist, können keine Postfachüberwachungsprotokolleinträge im Unterordner "Audits" im Ordner "Wiederherstellbare Elemente" gespeichert werden.

Für Postfächer, die nicht im Haltebereich sind, können Administratoren den `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Befehl in Exchange Online PowerShell verwenden, um Elemente im Ordner "Wiederherstellbare Elemente" zu löschen. Weitere Informationen finden Sie in den folgenden Themen:

- [Suchen nach und Löschen von Nachrichten](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Für Postfächer, die im Haltebereich sind, müssen Administratoren den Haltebereich entfernen, bevor sie Elemente aus dem Ordner "Wiederherstellbare Elemente" löschen können. Weitere Informationen finden [Sie unter "Löschen von Elementen im Ordner "Wiederherstellbare Elemente" von cloudbasierten Postfächern im Haltebereich](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Um zu verhindern, dass der Ordner "Wiederherstellbare Elemente" voll wird, können Administratoren die Speichergrenze des Ordners "Wiederherstellbare Elemente" für Postfächer im Haltebereich erhöhen und eine Aufbewahrungsrichtlinie für Postfächer einrichten, die Elemente aus dem Ordner "Wiederherstellbare Elemente" in das Archivpostfach des Benutzers verschiebt. Siehe [Erhöhen des Kontingents für wiederherstellbare Elemente für Postfächer im Haltebereich](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
