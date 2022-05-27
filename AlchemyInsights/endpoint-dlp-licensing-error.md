---
title: Endpunkt-DLP-Lizenzierungsfehler
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 2b5a65dae6f53bb89882d8426ab670cd200ba914
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65709410"
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
