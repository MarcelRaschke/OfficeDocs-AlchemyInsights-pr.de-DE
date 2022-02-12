---
title: Deaktivieren der Netzwerküberprüfung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: a7eb5daf4528df2ab07c518321a231de39a7ee00
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62669875"
---
# <a name="disable-network-scan"></a>Deaktivieren der Netzwerküberprüfung

Netzwerkfreigabeüberprüfungen können sich auf die Leistung auswirken.  Um sicherzustellen, dass der Client keine Netzwerkfreigaben/Dateien standardmäßig überprüft, konfigurieren Sie die folgenden Einstellungen in der Windows Defender-Anwendung auf **"True"**:

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles