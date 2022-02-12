---
title: Microsoft Edge Datenschutzeinstellungen konfigurieren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 83f39613a1274b358353eeaa9d88e09b749820b4
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62720277"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge Datenschutzeinstellungen konfigurieren

Wenn Microsoft Edge auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen standardmäßig nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch auf Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen gemäß [den Einstellungen Windows Diagnosedaten](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization) des Benutzers gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation behandelt:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Diese Richtlinie ermöglicht die Berichterstellung von Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Diese Richtlinie sendet Websiteinformationen, die verwendet werden, um Microsoft-Dienste zu verbessern.

Weitere Informationen finden Sie unter [Konfigurieren von Richtlinieneinstellungen](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).