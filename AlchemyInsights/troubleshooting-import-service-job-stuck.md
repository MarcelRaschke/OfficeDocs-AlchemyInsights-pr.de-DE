---
title: Problembehandlung Import-Serviceauftrag steckt fest
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003046"
- "7907"
ms.date: 04/27/2021
ms.openlocfilehash: 243a286ebce70cd414d4a4cec7c7af673190fc07
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66371199"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Problembehandlung Import-Serviceauftrag steckt fest

Wenn Sie Probleme mit steckengebliebenen oder fehlgeschlagenen Import-Service-Jobs haben, prüfen Sie und versuchen Sie Folgendes:

- Überprüfen Sie die Größe der PST-Datei. Die maximal empfohlene Größe einer PST-Datei für den Import beträgt 20 GB.

- Wenn Sie vermuten, dass Elemente aufgrund einer Beschädigung übersprungen wurden, führen Sie Scanpst.exe aus, um Fehler in PST-Dateien zu diagnostizieren und zu beheben.

- Wenn Sie während des Imports die Fehlermeldung "MapiExceptionShutoffQuotaExceeded" sehen, stellen Sie sicher, dass das Zielpostfach genügend Kapazität hat, um die gewünschten PST-Dateien zu importieren.

Weitere Informationen zur Problembehandlung bei PST-Importaufträgen finden Sie unter [Behebung von Problemen mit PST-Importaufträgen](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Informationen darüber, wie Probleme beim Importieren von PST-Dateien in Outlook behoben werden können, finden Sie unter [Probleme beim Importieren einer Outlook-.pst-Datei beheben (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).