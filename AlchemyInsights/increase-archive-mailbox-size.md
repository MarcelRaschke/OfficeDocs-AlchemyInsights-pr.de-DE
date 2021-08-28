---
title: 305 Erhöhen der Größe des Archivpostfachs
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926387"
---
# <a name="increase-the-archive-mailbox-size"></a>Erhöhen der Größe des Archivpostfachs


Wenn Sie möchten, dass wir automatisierte Überprüfungen für die unten genannten Einstellungen ausführen, wählen Sie die Schaltfläche "Zurück" < - oben auf dieser Seite aus, und geben Sie dann die E-Mail-Adresse des Benutzers ein, der die Größe des Archivpostfachs erhöhen muss.

Microsoft 365 [beschränkt](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) die Größe von Archivpostfächern basierend auf der Lizenz, die dem Benutzerkonto zugewiesen ist. Wenn das Archivpostfach 90 % seiner zulässigen Größe erreicht, erhält der Benutzer eine E-Mail-Benachrichtigung. Wenn ein Archivpostfach seine Größenbeschränkung erreicht, kann der Benutzer nicht mehr Elemente in das Archivpostfach verschieben. Microsoft 365 wird die Größe eines Archivpostfachs nicht erhöhen, sobald das Größenlimit erreicht ist. Stattdessen können Benutzer die folgenden Aktionen ausführen, um Speicherplatz im Archivpostfach freizugeben:

- Exportieren Sie die Elemente mit Outlook in eine PST-Datei.

- Löschen sie Elemente aus dem Archivpostfach.

Microsoft 365 bietet **eine unbegrenzte Archivierung** für Office 365 Enterprise E3- und E5-Lizenzen. Ein Administrator muss dieses Feature aktivieren, bevor das Archivpostfach seine maximale Größe erreicht. Wenn die unbegrenzte Archivierung aktiviert ist, kann es bis zu 30 Tage dauern, bis dem Archivpostfach freier Speicherplatz hinzugefügt wird. Daher wird empfohlen, dass Administratoren den freien Speicherplatz im Archivpostfach überprüfen, sodass der Benutzer das Archivpostfach weiterhin verwenden kann, während es erweitert wird. Weitere Informationen finden Sie unter [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and Enable unlimited archiving in [Microsoft 365.](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)

Weitere Informationen zum Zugriff auf das Archivpostfach über Outlook finden Sie unter [Outlook Anforderungen für den Zugriff auf Elemente in einem automatisch erweiterten Archiv.](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) Informationen zum Konfigurieren einer Aufbewahrungsrichtlinie, die Elemente automatisch in das Archivpostfach verschiebt, finden Sie unter [Einrichten einer Archivierungs- und Löschrichtlinie für Postfächer in Ihrer Microsoft 365 Organisation.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**Hinweis:** Automatisch erweiternde Archive werden für primäre Postfächer in Exchange 2010 nicht unterstützt.
