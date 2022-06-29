---
title: Einstellung von Access-Diensten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000356"
- "2009"
ms.openlocfilehash: 8d4ae591a449e58986ec081339ab5fd82fa92a2d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66314463"
---
# <a name="access-services-retirement"></a>Einstellung von Access-Diensten

Wie wir ursprünglich in MC97576 im März 2017 angekündigt haben und im vergangenen Jahr weiterhin kommuniziert haben, werden Access Services eingestellt. Die nächste Phase dieses Prozesses wird das Entfernen von Access-Webdatenbanken sein, die SharePoint-Listen als zugrunde liegenden Datenspeicher verwenden.

**Wie wirkt sich das auf mich aus?**

Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden Apps bis April 2020 beenden.

**Was muss ich als Vorbereitung auf diese Veränderung tun?**

Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen. Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der Access-Apps abzurufen, die von Websites verwendet werden.

Es gibt mehrere Möglichkeiten zum Migrieren von Access-Webdatenbankdaten:

- Importieren in eine lokale Access-Datenbank (. ACCDB) oder an eine Excel-Datei an.
- Wir empfehlen auch, Microsoft PowerApps als alternative Plattform zu erkunden, um codefreie Geschäftslösungen für Web- und Mobile-Geräte zu erstellen.