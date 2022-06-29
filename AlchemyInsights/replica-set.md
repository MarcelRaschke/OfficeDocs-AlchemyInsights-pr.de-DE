---
title: Replikatsatz
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: b96d03ef583f05da6c325be98525e5d1ce6472c7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66418517"
---
# <a name="replica-set"></a>Replikatsatz

AADDS wird auch als verwaltete Domäne bezeichnet. Es handelt sich tatsächlich um zwei Domänencontroller, die vom Back-End ausgeführt und verwaltet werden. Die beiden DCs umfassen einen Haupt-DC und einen Replikations-DC. Sicherungen in AADDS (verwaltete Domäne) sind ein automatisierter Prozess, der von der Azure-Plattform verwaltet wird. Im Falle eines Problems mit Ihrer verwalteten Domäne können Azure-Support Sie bei der Wiederherstellung aus der Sicherung unterstützen.

Sie erstellen jeden Replikatsatz in einem virtuellen Netzwerk. Jedes virtuelle Netzwerk muss mit jedem anderen virtuellen Netzwerk, das die Replikatgruppe einer verwalteten Domäne hostet, peered sein. Diese Konfiguration erstellt eine Gitternetzwerktopologie, die die Verzeichnisreplikation unterstützt. Ein virtuelles Netzwerk kann mehrere Replikatgruppen unterstützen, vorausgesetzt, dass sich jede Replikatgruppe in einem anderen virtuellen Subnetz befindet.

Weitere Informationen zu Replikatgruppen finden Sie unter [Konzepte von Replikatsätzen](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
