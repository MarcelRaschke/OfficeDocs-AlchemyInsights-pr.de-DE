---
title: Defender-Endpunkt – Überprüfen Sie den Sensorstatus
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: 2e758768442ea556b3e119de173de79dd43fdc35
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61938403"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender-Endpunkt – Überprüfen Sie den Sensorstatus

Die Kachel **Geräte mit Sensorproblemen** befindet sich auf dem Dashboard "Sicherheitsvorgänge". Diese Kachel enthält Informationen über die Kapazität des einzelnen Geräts, Sensordaten zu liefern und mit dem Defender für Endpunkt-Dienst zu kommunizieren. Sie zeigt an, wie viele Geräte Ihrer Aufmerksamkeit erfordern und hilft Ihnen, problematische Geräte zu identifizieren und Maßnahmen zur Behebung bekannter Probleme zu ergreifen.

Zwei Statusindikatoren auf der Kachel enthalten Informationen zur Anzahl der Geräte, die nicht ordnungsgemäß an den Dienst gemeldet werden:

- **Falsch konfigurierte** Geräte, die sensorische Daten möglicherweise nur teilweise beim Defender für Endpunkt-Dienst melden bzw. Konfigurationsfehler haben, die behoben werden müssen.
- **Inaktive** Geräte, die seit mehr als sieben Tagen im letzten Monat keine Meldungen mehr an den Defender für Endpunkt-Dienst gesendet haben.

Wenn Sie auf eine der Gruppen klicken, werden Sie zur Liste "Geräte" umgeleitet, die entsprechend Ihrer Auswahl gefiltert ist. In der Liste "Geräte" können Sie die Liste des Integritätsstatus nach dem folgenden Status filtern:

- **Aktive** Geräte, die aktiv Meldungen an den Defender für Endpunkt-Dienst senden.
- **Falsch konfigurierte** Geräte, die sensorische Daten möglicherweise nur teilweise beim Defender für Endpunkt-Dienst melden, die jedoch Konfigurationsfehler haben, die behoben werden müssen. Falsch konfigurierte Geräte können entweder eins oder eine Mischung aus den folgenden Probleme haben:

    - Keine Sensordaten – Die Geräte haben aufgehört, Sensordaten zu senden. Das Gerät kann begrenzt Alarme auslösen.
    - Beeinträchtigte Kommunikation – Die Fähigkeit, mit dem Gerät zu kommunizieren, ist beeinträchtigt. Dateien zur tiefen Analyse senden, Dateien sperren, das Gerät vom Netzwerk isolieren und andere Aktionen, die eine Kommunikation mit dem Gerät erfordern, funktionieren möglicherweise nicht.
- **Inaktive** Geräte, die keine Meldungen an den Defender für Endpunkt-Dienst mehr senden.

Sie können die gesamte Liste im CSV-Format mithilfe der Exportfunktion herunterladen.

Weitere Informationen finden Sie unter [Überprüfen des Integritätsstatus des Sensor in Microsoft Defender für Endpunkt](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status).

Weitere Informationen darüber, was dazu geführt hat, dass ein Gerät inaktiv oder falsch konfiguriert war, finden Sie unter [Beheben fehlerhafter Sensoren in Microsoft Defender für Endpunkt](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
