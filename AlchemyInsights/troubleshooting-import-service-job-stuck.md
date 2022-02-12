---
title: Problembehandlung Import-Serviceauftrag steckt fest
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 96aebdbf884e2acea245d9f000f685c138cee014
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62749583"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Problembehandlung Import-Serviceauftrag steckt fest

Wenn Sie Probleme mit steckengebliebenen oder fehlgeschlagenen Import-Service-Jobs haben, prüfen Sie und versuchen Sie Folgendes:

- Überprüfen Sie die Größe der PST-Datei. Die maximal empfohlene Größe einer PST-Datei für den Import beträgt 20 GB.

- Wenn Sie vermuten, dass Elemente aufgrund einer Beschädigung übersprungen wurden, führen Sie Scanpst.exe aus, um Fehler in PST-Dateien zu diagnostizieren und zu beheben.

- Wenn Sie während des Imports die Fehlermeldung "MapiExceptionShutoffQuotaExceeded" sehen, stellen Sie sicher, dass das Zielpostfach genügend Kapazität hat, um die gewünschten PST-Dateien zu importieren.

Weitere Informationen zur Problembehandlung bei PST-Importaufträgen finden Sie unter [Behebung von Problemen mit PST-Importaufträgen](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Informationen darüber, wie Probleme beim Importieren von PST-Dateien in Outlook behoben werden können, finden Sie unter [Probleme beim Importieren einer Outlook-.pst-Datei beheben (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).