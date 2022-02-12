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
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 25b59f7b8dc6416fa7d7ab96ec02fe5b90d1b78d
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62694644"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Einschränken SharePoint Online auf den klassischen Modus

Einige Organisationen benötigen weiterhin den klassischen Modus. Es gibt zwar keine Pläne, den klassischen Modus auf granularer Ebene zu entfernen, es ist jedoch nicht mehr möglich, eine gesamte Organisation (mandant) auf den klassischen Modus für Listen und Bibliotheken zu beschränken.

Der Administrator verfügt über die folgenden Optionen zum Verwalten einzelner Listen und Bibliotheken im klassischen Modus mit granularen Opt-Out-Switches, die wir auf den folgenden Ebenen bereitstellen:

- Websitesammlung
- Website
- Liste
- Bibliothek

Darüber hinaus werden Listen, die bestimmte Features und Anpassungen verwenden, die nicht von der modernen Version unterstützt werden, weiterhin automatisch in den klassischen Modus umgeschaltet.

Ab dem 1. April 2019 wird der Prozess zum Deaktivieren der Deaktivierung von modernen Listen und Bibliotheken auf Mandantenebene gestartet und bis zum 31. Mai 2019 fortgesetzt.  Die Listen und Bibliotheken, die sich aufgrund des Mandanten-Opt-Outs im klassischen Modus befinden, werden automatisch auf modern umgestellt.

Wenn Sie den klassischen Modus benötigen, finden Sie [hier](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) weitere Informationen und eine PnP Powershell-Anweisung [,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) die Optionen und Tools beschreibt, die Sie heute für die Verwendung der klassischen Modusumgebung verwenden können.
