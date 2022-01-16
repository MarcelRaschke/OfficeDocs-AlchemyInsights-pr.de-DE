---
title: Leistungsprobleme bei Microsoft Defender für Endpunkt unter Linux
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: fadaee10270141ffab731fe57bc5de5e301815c2
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61980778"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Leistungsprobleme bei Microsoft Defender für Endpunkt unter Linux

Dieser Artikel führt Sie durch die Schritte zum Identifizieren von Leistungsproblemen bei Microsoft Defender für Endpunkt unter Linux.

Es ist wichtig zuerst zu überprüfen, ob das Problem mit der [aktuellsten Version](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-whatsnew) behoben wurde. 

Informationen zum Starten Ihrer Untersuchung finden Sie unter [Behandeln von Leistungsproblemen bei Microsoft Defender für Endpunkt unter Linux](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Ausschlüsse

Ausschlüsse können zur Entschärfung von Leistungsproblemen beitragen. Überprüfen Sie Ihre Ausschlüsse, bevor Sie beginnen, damit zusätzliche Risiken bekannt und dokumentiert sind.

Weitere Informationen finden Sie unter [Konfigurieren und Überprüfen von Ausschlüssen für Microsoft Defender für Endpunkt unter Linux](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-exclusions).

Wenn Sie mehrere Dateien und Ordner ausschließen möchten und diese sich alle am selben Bereitstellungspunkt befinden, könnte es einfacher sein, den Bereitstellungspunkt auszuschließen. Beginnend mit der Februar-Version 101.22.80 können Sie einen gesamten Bereitstellungspunkt ausschließen.

Wenn z. B. "/mnt/backup" ein Bereitstellungspunkt ist, können Sie der Ausschlussliste "/mnt/backup" hinzufügen, indem Sie den folgenden Befehl ausführen:

`$ mdatp exclusion folder add –path /mnt/backup`

**Hinweis**: Durch das Hinzufügen von Ausschlüssen erhöht sich das Risiko, dass Schadsoftware nicht erkannt wird. Das Ausschließen sollte mit Bedacht eingesetzt werden.

## <a name="need-help"></a>Benötigen Sie Hilfe?

Sammeln Sie die Diagnosedaten, bevor Sie einen Supportfall öffnen, damit wir Ihnen so effizient wie möglich helfen können.
