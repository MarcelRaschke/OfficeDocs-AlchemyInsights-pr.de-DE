---
title: Einschränken SharePoint Online auf den klassischen Modus
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: eb008d7a764fb0e2d135b8f673ce4574158762b4
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65732396"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Einschränken SharePoint Online auf den klassischen Modus

Einige Organisationen benötigen weiterhin die Oberfläche für den klassischen Modus. Es gibt zwar keine Pläne, den klassischen Modus auf granularer Ebene zu entfernen, es ist jedoch nicht mehr möglich, eine gesamte Organisation (mandant) auf den klassischen Modus für Listen und Bibliotheken zu beschränken.

Der Administrator hat die folgenden Optionen, um einzelne Listen und Bibliotheken im klassischen Modus mithilfe präziser Opt-Out-Switches zu verwalten, die wir auf den folgenden Ebenen bereitstellen:

- Websitesammlung
- Website
- Liste
- Bibliothek

Darüber hinaus werden Listen, die bestimmte Features und Anpassungen verwenden, die nicht von modern unterstützt werden, weiterhin automatisch in den klassischen Modus umgeschaltet.

Ab dem 1. April 2019 wird der Prozess zum Deaktivieren der Deaktivierung der Mandantenebene für moderne Listen und Bibliotheken bis zum 31. Mai 2019 gestartet und fortgesetzt.  Die Listen und Bibliotheken, die sich im klassischen Modus als Ergebnis der Mandanten-Deaktivierung befinden, werden automatisch auf modern umgestellt.

Wenn Sie den klassischen Modus benötigen, finden Sie [hier](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) weitere Informationen und [hier](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) eine PnP PowerShell-Anweisung, die Optionen und Tools beschreibt, die Sie heute für die Verwendung des klassischen Modus verwenden können.
