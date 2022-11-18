---
title: Konfigurieren von Datenschutzeinstellungen in Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003843"
- "6892"
ms.date: 12/03/2020
ms.openlocfilehash: d0ea7a4c285fcb278e0575fee5266d41d4d23836
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66403564"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Konfigurieren von Datenschutzeinstellungen in Microsoft Edge

Wenn Microsoft Edge auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen standardmäßig nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch auf Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen entsprechend den [Windows-Diagnosedateneinstellungen](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization) der Benutzer gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation behandelt:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Diese Richtlinie ermöglicht die Berichterstellung über Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Diese Richtlinie sendet Websiteinformationen, die verwendet werden, um Microsoft-Dienste zu verbessern.

Weitere Informationen finden Sie [unter Konfigurieren von Richtlinieneinstellungen](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).