---
title: Gerät aktivieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 568f415953b68f2787ba8398567ee6bb7c61af96
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66391467"
---
# <a name="enable-device"></a>Gerät aktivieren

**So aktivieren Sie das Gerät mithilfe des Powershell-Befehls**

Führen Sie die folgenden Befehle aus:

- So rufen Sie das Geräteobjekt ab: `Get-MsolDevice -Name <Name>`
- So aktivieren Sie das Gerät: `Enable-MsolDevice -DeviceId <DeviceId>`

Weitere Informationen zum Konfigurieren der Hybridbeitrittsfunktion für verwaltete Domänen finden [Sie unter Konfigurieren der Hybridbeitrittsfunktion](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
