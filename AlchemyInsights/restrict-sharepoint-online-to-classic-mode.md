---
title: Einschränken von SharePoint Online auf den klassischen Modus
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000225"
- "1835"
- "1889"
ms.date: 04/21/2020
ms.openlocfilehash: ec7929775e9c7987b7a5d5f97ec44fa708eaaf8c
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66264071"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Einschränken von SharePoint Online auf den klassischen Modus

Einige Organisationen benötigen weiterhin die Oberfläche für den klassischen Modus. Es gibt zwar keine Pläne, den klassischen Modus auf granularer Ebene zu entfernen, es ist jedoch nicht mehr möglich, eine gesamte Organisation (mandant) auf den klassischen Modus für Listen und Bibliotheken zu beschränken.

Der Administrator hat die folgenden Optionen, um einzelne Listen und Bibliotheken im klassischen Modus mithilfe präziser Opt-Out-Switches zu verwalten, die wir auf den folgenden Ebenen bereitstellen:

- Websitesammlung
- Website
- Liste
- Bibliothek

Darüber hinaus werden Listen, die bestimmte Features und Anpassungen verwenden, die nicht von modern unterstützt werden, weiterhin automatisch in den klassischen Modus umgeschaltet.

Ab dem 1. April 2019 wird der Prozess zum Deaktivieren der Deaktivierung der Mandantenebene für moderne Listen und Bibliotheken bis zum 31. Mai 2019 gestartet und fortgesetzt.  Die Listen und Bibliotheken, die sich im klassischen Modus als Ergebnis der Mandanten-Deaktivierung befinden, werden automatisch auf modern umgestellt.

Wenn Sie den klassischen Modus benötigen, finden Sie [hier](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) weitere Informationen und [hier](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) eine PnP PowerShell-Anweisung, die Optionen und Tools beschreibt, die Sie heute für die Verwendung des klassischen Modus verwenden können.
