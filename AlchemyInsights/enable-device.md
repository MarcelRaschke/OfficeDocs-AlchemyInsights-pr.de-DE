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
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003482"
---
# <a name="enable-device"></a>Gerät aktivieren

**So aktivieren Sie das Gerät mithilfe des PowerShell-Befehls**

Führen Sie die folgenden Befehle aus:

- So rufen Sie das Geräteobjekt ab: `Get-MsolDevice -Name <Name>`
- So aktivieren Sie das Gerät: `Enable-MsolDevice -DeviceId <DeviceId>`

Weitere Informationen zum Konfigurieren des Hybridbeitritts in verwalteten Domänen finden Sie unter Konfigurieren des [Hybridbeitritts.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
