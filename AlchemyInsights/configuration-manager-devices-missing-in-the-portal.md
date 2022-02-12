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
ms.openlocfilehash: 0525799e6fc3278e0bdbb74dce489b87ae91b803
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62557397"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Im-Portal fehlen Configuration Manager-Geräte

Damit die Gerätesynchronisierung funktioniert, müssen die [erforderlichen Internet Endpunkte](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) über den lokalen Server erreichbar sein, auf dem die Rolle "Dienstverbindungspunkt" gehostet wird. Informationen zur Problembehandlung bei der Synchronisierung von Geräten finden Sie im **CMGatewaySyncUploadWorker.log**, das sich im Dienstverbindungspunkt befindet.

Erfahren Sie mehr über das [Anfügen von Mandanten in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
