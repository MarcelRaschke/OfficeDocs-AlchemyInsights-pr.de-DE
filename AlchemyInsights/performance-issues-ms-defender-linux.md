---
title: Leistungsprobleme bei Microsoft Defender für Endpunkt unter Linux
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9001464"
- "11491"
ms.date: 06/04/2021
ms.openlocfilehash: 77be222a8a1fc63e6b04cfa7a692a7469e6d12f0
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66305766"
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

`$ mdatp exclusion folder add -path /mnt/backup`

**Hinweis**: Durch das Hinzufügen von Ausschlüssen erhöht sich das Risiko, dass Schadsoftware nicht erkannt wird. Das Ausschließen sollte mit Bedacht eingesetzt werden.

## <a name="need-help"></a>Benötigen Sie Hilfe?

Sammeln Sie die Diagnosedaten, bevor Sie einen Supportfall öffnen, damit wir Ihnen so effizient wie möglich helfen können.
