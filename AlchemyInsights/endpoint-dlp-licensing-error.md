---
title: Endpunkt-DLP-Lizenzierungsfehler
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3200001"
- "7176"
ms.date: 11/23/2020
ms.openlocfilehash: b4a82afcb098b4a5e07c5b8bfbf7001255b5d6c9
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66297604"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpunkt-DLP-Lizenzierungsfehler

Wenn Sie versuchen, Endpunkt-DLP einzurichten, wenn dieser Fehler angezeigt wird:

`Your organization is missing the licenses required to manage these devices.`

Stellen Sie sicher, dass Sie über eines der folgenden Abonnements oder Add-Ons verfügen:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Compliance
- Microsoft 365 A5 Compliance
- Microsoft 365 E5 Information Protection und Governance
- Microsoft 365 A5 Information Protection und Governance

**Hinweis**: Dies funktioniert nicht für Lizenzkombinationen wie: Win E5 + O365 E5 + EMS E5. Sie müssen über eine reine Microsoft 365 E5 Lizenz verfügen, um dieses Feature einzurichten.

Weitere Informationen zur Endpunkt-DLP-Lizenzierung finden Sie unter [Endpunkt-DLP-Lizenzierung.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
