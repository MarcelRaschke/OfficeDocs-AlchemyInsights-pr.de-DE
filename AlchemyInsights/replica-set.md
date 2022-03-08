---
title: Replikatsatz
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: bbee442cb34fc4ce072c9cc68aa0c28d7c8b3623
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63222729"
---
# <a name="replica-set"></a>Replikatsatz

AADDS wird auch als verwaltete Domäne bezeichnet. Es handelt sich tatsächlich um zwei Domänencontroller, die vom Back-End ausgeführt und verwaltet werden. Die beiden DCs enthalten einen Haupt-DC und einen Replikations-DC. Sicherungen in AADDS (verwaltete Domäne) sind ein automatisierter Prozess, der von der Azure-Plattform verwaltet wird. Im Falle eines Problems mit Ihrer verwalteten Domäne kann der Azure-Support Sie bei der Wiederherstellung aus der Sicherung unterstützen.

Sie erstellen jede Replikatgruppe in einem virtuellen Netzwerk. Jedes virtuelle Netzwerk muss mit jedem anderen virtuellen Netzwerk gepeert werden, das die Replikatgruppe einer verwalteten Domäne hostet. Diese Konfiguration erstellt eine Gitternetzwerktopologie, die die Verzeichnisreplikation unterstützt. Ein virtuelles Netzwerk kann mehrere Replikatgruppen unterstützen, vorausgesetzt, jede Replikatgruppe befindet sich in einem anderen virtuellen Subnetz.

Weitere Informationen zur Replikatgruppe finden Sie unter ["Konzepte für Replikatgruppen"](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
