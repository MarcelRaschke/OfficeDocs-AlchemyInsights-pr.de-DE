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
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 336fae2c6b9628be66681de298b643b7ef26fb86
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62701988"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurieren von Datenschutzeinstellungen in Microsoft Edge

Wenn Microsoft Edge standardmäßig auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch auf Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen gemäß [den Diagnosedateneinstellungen der Benutzer Windows](https://go.microsoft.com/fwlink/?linkid=2132472) gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation behandelt:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiviert die Berichterstellung über Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sendet Websiteinformationen, die verwendet werden, um Microsoft-Dienste zu verbessern.

Weitere Informationen finden Sie unter [Konfigurieren von Richtlinieneinstellungen](https://go.microsoft.com/fwlink/?linkid=2132577).
