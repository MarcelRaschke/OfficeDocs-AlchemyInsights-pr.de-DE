---
title: Konfigurieren von Datenschutzeinstellungen in Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: bca782af04e53e8e5decc18276ddbb14638dfb60
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63267713"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurieren von Datenschutzeinstellungen in Microsoft Edge

Wenn Microsoft Edge auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen standardmäßig nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch auf Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen gemäß den [Einstellungen für diagnosedaten der Benutzer Windows](https://go.microsoft.com/fwlink/?linkid=2132472) gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation behandelt:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiviert die Berichterstellung über Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sendet Websiteinformationen, die verwendet werden, um Microsoft-Dienste zu verbessern.

Weitere Informationen finden Sie unter [Konfigurieren von Richtlinieneinstellungen](https://go.microsoft.com/fwlink/?linkid=2132577).
