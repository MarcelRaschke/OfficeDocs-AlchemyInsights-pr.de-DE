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
ms.openlocfilehash: 15d86de954f25d40b00f6b5e5c9a3f9f9ace4643
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65730486"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuelle Konfiguration mit AAD Domain Services

Die virtuelle Konfiguration mit AAD Domain Services umfasst die folgenden Schritte: 

1. Überprüfen des Zustands Ihrer Domäne im Azure-Portalhttps://aka.ms/aadds-health
2. Überprüfen Ihres NSG auf Regeln, die Ports blockieren, die für die Synchronisierung in den Azure AD Domain Services im Portal https://aka.ms/aadds-networking erforderlich sind.
3. Sicherstellen, dass Ihr virtuelles Netzwerk in derselben Azure-Region wie die von Azure AD Domain Services verwaltete Domäne bereitgestellt wird.
4. Stellen Sie sicher, dass Sie keine vorhandene Domäne mit demselben Domänennamen haben, die im virtuellen Netzwerk verfügbar ist.

Weitere Details zu Designüberlegungen zum virtuellen Netzwerk von Azure zur Unterstützung von AAD Domain Services finden Sie unter [Überlegungen zum virtuellen Netzwerk](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

