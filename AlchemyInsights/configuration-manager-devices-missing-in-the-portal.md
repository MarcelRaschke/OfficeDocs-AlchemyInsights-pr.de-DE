---
title: Im-Portal fehlen Configuration Manager-Geräte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966108"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Im-Portal fehlen Configuration Manager-Geräte

Damit die Gerätesynchronisierung funktioniert, müssen die [erforderlichen Internet Endpunkte](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) über den lokalen Server erreichbar sein, auf dem die Rolle "Dienstverbindungspunkt" gehostet wird. Informationen zur Problembehandlung bei der Synchronisierung von Geräten finden Sie im **CMGatewaySyncUploadWorker.log**, das sich im Dienstverbindungspunkt befindet.

Erfahren Sie mehr über das [Anfügen von Mandanten in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
