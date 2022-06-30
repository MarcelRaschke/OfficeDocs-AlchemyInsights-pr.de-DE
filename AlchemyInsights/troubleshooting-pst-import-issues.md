---
title: Behandlung von Problemen beim PST-Import
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 95590dc8bee3dd67e127bdb7e2faa05662d5c60b
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66333741"
---
# <a name="troubleshooting-pst-import-issues"></a>Behandlung von Problemen beim PST-Import

- Wenn Sie innerhalb des Outlook-Clients selbst importieren, siehe [Probleme beim Importieren einer Outlook-.pst-Datei beheben](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Wenn Sie den Importdienst verwenden und dieser feststeckt, beachten Sie, dass jede PST-Datei, die Sie auf Azure-Storage hochladen, nicht größer als 20 GB sein sollte. PST-Dateien mit mehr als 20 GB können sich auf die Leistung des PST-Importprozesses auswirken. Weitere Informationen zur Problembehandlung bei festhängenden Aufträgen finden Sie unter [Probleme, die PST-Importaufträge betreffen](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Wenn Sie den Status eines bestimmten Importauftrags überprüfen möchten, verwenden Sie [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Ausführliche Informationen zum Importdienst finden Sie unter [Übersicht über das Importieren von PST-Dateien Ihrer Organisation](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365).
