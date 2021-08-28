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
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072843"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuelle Konfiguration mit AAD Domain Services

Die virtuelle Konfiguration mit AAD Domain Services umfasst die folgenden Schritte: 

1. Überprüfen des Integritätszustands Ihrer Domäne im Azure-Portal https://aka.ms/aadds-health.
2. Überprüfen Ihres NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in den Azure AD Domain Services im Portal https://aka.ms/aadds-networking erforderlich sind.
3. Sicherstellen, dass Ihr virtuelles Netzwerk in derselben Azure-Region wie die von Azure AD Domain Services verwaltete Domäne bereitgestellt wird.
4. Sicherstellen, dass Sie nicht über eine vorhandene Domäne mit demselben Domänennamen verfügen, die im virtuellen Netzwerk verfügbar ist.

Weitere Details zu Designüberlegungen zum virtuellen Netzwerk von Azure zur Unterstützung von AAD Domain Services finden Sie unter [Überlegungen zum virtuellen Netzwerk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

