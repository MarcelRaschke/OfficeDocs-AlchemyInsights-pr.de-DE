---
title: Ausmusterung von Access-Diensten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 111be4924be9d03747f590ef4296b0a6ee10dcab
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63288521"
---
# <a name="access-services-retirement"></a>Ausmusterung von Access-Diensten

Wie ursprünglich in MC97576 angekündigt, wurden im März 2017 die Access Services eingestellt und die Kommunikation im letzten Jahr fortgesetzt. Die nächste Phase in diesem Prozess ist das Entfernen von Access-Webdatenbanken, die SharePoint-Listen als zugrunde liegende Datenspeicherung verwenden.

**Wie wirkt sich das auf mich aus?**

Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden Apps bis April 2020 herunterfahren.

**Was muss ich als Vorbereitung auf diese Veränderung tun?**

Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen. Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der von Websites verwendeten Access-Apps zu erhalten.

Es gibt mehrere Möglichkeiten zum Migrieren von Access-Webdatenbankdaten:

- Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.
- Wir empfehlen außerdem, Microsoft PowerApps als alternative Plattform zu erkunden, um codelose Geschäftslösungen für Web- und mobile Geräte zu erstellen.