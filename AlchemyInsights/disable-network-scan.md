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
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 5bac23822d7b284a274dac79e3328a268af793fa
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63215853"
---
# <a name="disable-network-scan"></a>Deaktivieren der Netzwerküberprüfung

Netzwerkfreigabeüberprüfungen können sich auf die Leistung auswirken.  Um sicherzustellen, dass der Client keine Netzwerkfreigaben/Dateien standardmäßig überprüft, konfigurieren Sie die folgenden Einstellungen in der Windows Defender-Anwendung auf **"True"**:

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles