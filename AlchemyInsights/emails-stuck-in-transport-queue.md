---
title: 'Neu auftretendes Problem: E-Mails hängen in Transportwarteschlangen'
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "3100010"
- "16270"
ms.openlocfilehash: 2d85024103bb43170c5684320b0e7afad92d0bc1
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66298261"
---
# <a name="emerging-issue-email-stuck-in-transport-queues"></a>Neu auftretendes Problem: E-Mails hängen in Transportwarteschlangen

Sie können beobachten, wie sich E-Mails in Exchange Server 2016- und Exchange Server 2019-Transportwarteschlangen aufbauen. Um das Problem zu lösen, laden Sie ein Skript auf jeden Exchange-Server in Ihrer Organisation herunter, und [führen Sie es aus](https://aka.ms/ResetScanEngineVersion) . Sie können das Skript auf mehreren Servern parallel ausführen.

Ausführliche Informationen finden Sie [unter "E-Mail stuck in Exchange On-premises Transport Queues](https://techcommunity.microsoft.com/t5/exchange-team-blog/email-stuck-in-exchange-on-premises-transport-queues/ba-p/3049447)".

Hinweise:  

- Führen Sie das Skript im Verwaltungsmodus aus.
- Die Ausführung des Skripts kann bis zu 30 bis 40 Minuten dauern.

Nach dem Ausführen des Skripts benötigt die Warteschlange Zeit zum Bereinigen. Sie können die Warteschlange mithilfe des Befehls "Get-Queue" überwachen.
