---
title: Im-Portal fehlen Configuration Manager-Geräte
ms.author: cmcatee
author: cmcatee-MSFT
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
ms.openlocfilehash: f940d384902898ca2ce747f820a63d936ba427ac
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61972041"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Im-Portal fehlen Configuration Manager-Geräte

Damit die Gerätesynchronisierung funktioniert, müssen die [erforderlichen Internet Endpunkte](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) über den lokalen Server erreichbar sein, auf dem die Rolle "Dienstverbindungspunkt" gehostet wird. Informationen zur Problembehandlung bei der Synchronisierung von Geräten finden Sie im **CMGatewaySyncUploadWorker.log**, das sich im Dienstverbindungspunkt befindet.

Erfahren Sie mehr über das [Anfügen von Mandanten in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
