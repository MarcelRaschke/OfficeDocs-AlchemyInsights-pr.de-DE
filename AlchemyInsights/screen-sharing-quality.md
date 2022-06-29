---
title: Bildschirmfreigabequalität
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002254"
- "9002536"
- "11061"
- "11062"
ms.date: 04/26/2021
ms.openlocfilehash: 49338787676ba6222a4a781295f5307bc8c4339f
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66347079"
---
# <a name="screen-sharing-quality"></a>Bildschirmfreigabequalität

In den meisten Fällen basieren Qualitätsprobleme bei der Bildschirmfreigabe zu einer begrenzten Bandbreite auf Clientseite.  Wenn die Bandbreite nicht begrenzt ist, wird Teams die Medienqualität optimieren, bis hin zu einer Videoauflösung von 1080 Pixel, 30 Bilder pro Sekunde (Frames per Second, FPS) für Video und 15 FPS für Inhalte sowie HiFi-Audio.

Microsoft Teams verhält sich hinsichtlich der Bandbreitennutzung immer konservativ und kann in weniger als 1,2 MBit/s High-Definition-Videoqualität bereitstellen. Die tatsächliche Bandbreitennutzung in den einzelnen Audio/Video-Anrufen oder Besprechungen variiert abhängig von Faktoren, wie z. B. Videolayout, Videoauflösung und Videoframes pro Sekunde. Wenn mehr Bandbreite verfügbar ist, werden Qualität und Nutzung erhöht, um die besten Ergebnisse zu erzielen. In dieser Tabelle wird veranschaulicht, wie Teams Bandbreite nutzt:

**Szenarien für die Bandbreite (mehr/ weniger)**

- 30 KBit/s Peer-to-Peer-Audioanrufe

- 130 KBit/s Peer-to-Peer-Audioanrufe und Bildschirmfreigabe

- 500 KBit/s Peer-to-Peer-Qualitätsvideoanrufe (360 Pixel bei 30 fps)

- 1,2 MBit/s Peer-to-Peer-Videoanrufe in HD-Qualität mit einer Auflösung von 720 Pixel bei 30 fps

- 1,5 MBit/s Peer-to-Peer-Videoanrufe in HD-Qualität mit einer Auflösung von 1080 Pixel bei 30 fps

- 500 KBit/s/ 1 MBit/s Gruppen-Videoanruf

- 1 MBit/s / 2 MBit/s Gruppenvideoanrufe in HD-Qualität (540 Pixel-Videos auf 1080 Pixel-Bildschirm)

Weitere Informationen finden Sie unter [Vorbereiten des Netzwerks Ihrer Organisation für Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements).