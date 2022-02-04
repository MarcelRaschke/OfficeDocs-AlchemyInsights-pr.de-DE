---
title: Ausmusterung von Access-Diensten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 9fa45a441600c01f24dd140712842fea21c70335
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61937107"
---
# <a name="access-services-retirement"></a>Ausmusterung von Access-Diensten

Wie ursprünglich in MC97576 im März 2017 angekündigt, kommunizierten wir im letzten Jahr weiterhin, Access Services eingestellt werden. Die nächste Phase in diesem Prozess ist das Entfernen von Access-Webdatenbanken, die SharePoint Listen als zugrunde liegende Datenspeicherung verwenden.

**Wie wirkt sich das auf mich aus?**

Ab Juni 2019 beenden wir die Erstellung neuer Access-Datenbanken in SharePoint Online und fahren den Dienst und alle verbleibenden Apps bis April 2020 herunter.

**Was muss ich als Vorbereitung auf diese Veränderung tun?**

Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen. Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der von Websites verwendeten Access-Apps zu erhalten.

Es gibt mehrere Möglichkeiten zum Migrieren von Access-Webdatenbankdaten:

- Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.
- Wir empfehlen außerdem, Microsoft PowerApps als alternative Plattform zu erkunden, um codelose Geschäftslösungen für Web- und mobile Geräte zu erstellen.