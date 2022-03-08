---
title: Virtuelle Konfiguration mit AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 61e08ab2927c95f15a8a5135b092aa39fbff590a
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63280781"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuelle Konfiguration mit AAD Domain Services

Die virtuelle Konfiguration mit AAD Domain Services umfasst die folgenden Schritte: 

1. Überprüfen des Integritätszustands Ihrer Domäne im Azure-Portal https://aka.ms/aadds-health.
2. Überprüfen Ihres NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in den Azure AD Domain Services im Portal https://aka.ms/aadds-networking erforderlich sind.
3. Sicherstellen, dass Ihr virtuelles Netzwerk in derselben Azure-Region wie die von Azure AD Domain Services verwaltete Domäne bereitgestellt wird.
4. Sicherstellen, dass Sie nicht über eine vorhandene Domäne mit demselben Domänennamen verfügen, die im virtuellen Netzwerk verfügbar ist.

Weitere Details zu Designüberlegungen zum virtuellen Netzwerk von Azure zur Unterstützung von AAD Domain Services finden Sie unter [Überlegungen zum virtuellen Netzwerk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

