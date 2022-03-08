---
title: Gerät aktivieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 7173a699ce65db46d41c3eae952172ec3a9472cb
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63248093"
---
# <a name="enable-device"></a>Gerät aktivieren

**So aktivieren Sie das Gerät mithilfe des PowerShell-Befehls**

Führen Sie die folgenden Befehle aus:

- So rufen Sie das Geräteobjekt ab: `Get-MsolDevice -Name <Name>`
- So aktivieren Sie das Gerät: `Enable-MsolDevice -DeviceId <DeviceId>`

Weitere Informationen zum Konfigurieren des Hybridbeitritts in verwalteten Domänen finden Sie unter [Konfigurieren der Hybrid-Verknüpfung](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
