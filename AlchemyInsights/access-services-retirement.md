---
title: Ausmusterung von Access-Diensten
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938694"
---
# <a name="access-services-retirement"></a>Ausmusterung von Access-Diensten

Wie ursprünglich in MC97576 im März 2017 angekündigt, kommunizierten wir im letzten Jahr weiterhin, Access Services eingestellt werden. Die nächste Phase in diesem Prozess ist das Entfernen von Access-Webdatenbanken, die SharePoint Listen als zugrunde liegende Datenspeicherung verwenden.

**Wie wirkt sich dies auf mich aus?**

Ab Juni 2019 beenden wir die Erstellung neuer Access-Datenbanken in SharePoint Online und beenden den Dienst und alle verbleibenden Apps bis April 2020.

**Was muss ich tun, um mich auf diese Änderung vorzubereiten?**

Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen. Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der von Websites verwendeten Access-Apps abzurufen.

Es gibt mehrere Möglichkeiten zum Migrieren von Access-Webdatenbankdaten:

- Importieren in eine lokale Access-Datenbank (. ACCDB) oder einer Excel-Datei.
- Wir empfehlen außerdem, Microsoft PowerApps als alternative Plattform zu untersuchen, um codelose Geschäftslösungen für Web- und mobile Geräte zu erstellen.