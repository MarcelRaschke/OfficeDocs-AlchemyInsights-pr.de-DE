---
title: Bildschirmfreigabequalität
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 266d2ee4fd3a96287c65ce70ad2b170e9cc5ab36
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860591"
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