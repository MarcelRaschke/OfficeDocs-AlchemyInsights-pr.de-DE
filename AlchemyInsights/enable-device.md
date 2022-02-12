---
title: Gerät aktivieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: af63ad13162cd10955c9b2d9a71e97d063d49311
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62653134"
---
# <a name="enable-device"></a>Gerät aktivieren

**So aktivieren Sie das Gerät mithilfe des PowerShell-Befehls**

Führen Sie die folgenden Befehle aus:

- So rufen Sie das Geräteobjekt ab: `Get-MsolDevice -Name <Name>`
- So aktivieren Sie das Gerät: `Enable-MsolDevice -DeviceId <DeviceId>`

Weitere Informationen zum Konfigurieren des Hybridbeitritts in verwalteten Domänen finden Sie unter [Konfigurieren der Hybrid-Verknüpfung](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
