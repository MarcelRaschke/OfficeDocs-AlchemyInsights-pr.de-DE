---
title: Konfigurieren von Datenschutzeinstellungen in Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004632"
- "8367"
ms.date: 03/24/2021
ms.openlocfilehash: bdafe0631bb1f61b92325747f5cb4e1826cd1dde
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66342237"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurieren von Datenschutzeinstellungen in Microsoft Edge

Wenn Microsoft Edge auf Nicht-Windows-Plattformen bereitgestellt wird, werden Diagnosedaten und Websiteinformationen standardmäßig nicht an Microsoft gesendet. Wenn Microsoft Edge jedoch auf Windows 10 bereitgestellt wird, werden Diagnosedaten und Websiteinformationen entsprechend den [Windows-Diagnosedateneinstellungen](https://go.microsoft.com/fwlink/?linkid=2132472) der Benutzer gesendet.

Verwenden Sie die folgenden Gruppenrichtlinien, um zu konfigurieren, wie Microsoft Edge die Datensammlung für Ihre Organisation behandelt:

- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) aktiviert die Berichterstellung über Nutzungs- und Absturzdaten.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sendet Websiteinformationen, die zur Verbesserung der Microsoft-Dienste verwendet werden.

Weitere Informationen finden Sie [unter Konfigurieren von Richtlinieneinstellungen](https://go.microsoft.com/fwlink/?linkid=2132577).
