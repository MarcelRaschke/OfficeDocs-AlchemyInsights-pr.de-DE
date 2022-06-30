---
title: Virtuelle Konfiguration mit AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004397"
- "7927"
ms.date: 01/15/2021
ms.openlocfilehash: 4c20a58fc050b494957e8cbb8d2e77fb974eb3fe
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66516036"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuelle Konfiguration mit AAD Domain Services

Die virtuelle Konfiguration mit AAD Domain Services umfasst die folgenden Schritte: 

1. Überprüfen des Zustands Ihrer Domäne im Azure-Portalhttps://aka.ms/aadds-health
2. Überprüfen Ihres NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in den Azure AD Domain Services im Portal https://aka.ms/aadds-networking erforderlich sind.
3. Sicherstellen, dass Ihr virtuelles Netzwerk in derselben Azure-Region wie die von Azure AD Domain Services verwaltete Domäne bereitgestellt wird.
4. Stellen Sie sicher, dass Sie keine vorhandene Domäne mit demselben Domänennamen haben, die im virtuellen Netzwerk verfügbar ist.

Weitere Details zu Designüberlegungen zum virtuellen Netzwerk von Azure zur Unterstützung von AAD Domain Services finden Sie unter [Überlegungen zum virtuellen Netzwerk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

