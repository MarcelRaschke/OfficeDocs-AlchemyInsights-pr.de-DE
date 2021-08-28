---
title: Replikatsatz
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110679"
---
# <a name="replica-set"></a>Replikatsatz

AADDS wird auch als verwaltete Domäne bezeichnet. Es handelt sich tatsächlich um zwei Domänencontroller, die vom Back-End ausgeführt und verwaltet werden. Die beiden DCs enthalten einen Haupt-DC und einen Replikations-DC. Sicherungen in AADDS (verwaltete Domäne) sind ein automatisierter Prozess, der von der Azure-Plattform verwaltet wird. Im Falle eines Problems mit Ihrer verwalteten Domäne kann der Azure-Support Sie bei der Wiederherstellung aus der Sicherung unterstützen.

Sie erstellen jede Replikatgruppe in einem virtuellen Netzwerk. Jedes virtuelle Netzwerk muss mit jedem anderen virtuellen Netzwerk gepeert werden, das die Replikatgruppe einer verwalteten Domäne hostet. Diese Konfiguration erstellt eine Gitternetzwerktopologie, die die Verzeichnisreplikation unterstützt. Ein virtuelles Netzwerk kann mehrere Replikatgruppen unterstützen, vorausgesetzt, jede Replikatgruppe befindet sich in einem anderen virtuellen Subnetz.

Weitere Informationen zur Replikatgruppe finden Sie unter ["Konzepte für Replikatgruppen".](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
