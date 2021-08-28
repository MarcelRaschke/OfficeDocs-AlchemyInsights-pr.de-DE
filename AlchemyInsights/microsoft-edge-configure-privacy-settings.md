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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114171"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge Datenschutzeinstellungen konfigurieren

Wenn Microsoft Edge auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen standardmäßig nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch auf Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen gemäß den Einstellungen für [diagnosedaten der](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)Benutzer Windows gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation behandelt:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)Diese Richtlinie ermöglicht die Berichterstellung von Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Diese Richtlinie sendet Websiteinformationen, die verwendet werden, um Microsoft-Dienste zu verbessern.

Weitere Informationen finden Sie unter [Konfigurieren von Richtlinieneinstellungen.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)