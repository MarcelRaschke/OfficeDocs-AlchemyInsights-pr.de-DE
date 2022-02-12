---
title: 'Neu auftretendes Problem: E-Mail bleibt in Transportwarteschlangen hängen'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100010"
- "16270"
ms.openlocfilehash: bb9e4e508285ade52068a3920531b4e44b2fca9c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62721333"
---
# <a name="emerging-issue-email-stuck-in-transport-queues"></a>Neu auftretendes Problem: E-Mail bleibt in Transportwarteschlangen hängen

Sie können den E-Mail-Aufbau in Exchange Server 2016 und Exchange Server 2019-Transportwarteschlangen beobachten. Um das Problem zu beheben, laden Sie ein Skript herunter, und [führen Sie es](https://aka.ms/ResetScanEngineVersion) auf jedem Exchange Server in Ihrer Organisation aus. Sie können das Skript parallel auf mehreren Servern ausführen.

Ausführliche Informationen finden Sie unter ["E-Mail stuck in Exchange On-premises Transport Queues"](https://techcommunity.microsoft.com/t5/exchange-team-blog/email-stuck-in-exchange-on-premises-transport-queues/ba-p/3049447).

Hinweise:  

- Führen Sie das Skript im Verwaltungsmodus aus.
- Die Ausführung des Skripts kann bis zu 30 bis 40 Minuten dauern.

Nach dem Ausführen des Skripts nimmt die Warteschlange Zeit für die Bereinigung in Anspruch. Sie können die Warteschlange mithilfe des Befehls "get-queue" überwachen.
