---
title: EndPoint Manager – Sicherheitsbasispläne
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 08d06e2589e70bef4ef360137e3cadded294316e
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62577624"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – Sicherheitsbasispläne

Sicherheitsbasispläne sind vorkonfigurierte Gruppen von Windows-Einstellungen, mit denen Sie die von den entsprechenden Sicherheitsteams empfohlenen Sicherheitseinstellungen anwenden können. Diese Basispläne können angepasst werden, um nur die gewünschten Einstellungen und Werte zu liefern. Weitere Informationen zu Sicherheitsbasispläne finden Sie unter [Verwenden von Sicherheitsbasispläne zum Konfigurieren von Windows 10-Geräten in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Derzeit gibt es Basispläne für diese Produkte:

- Windows MDM-Sicherheitseinstellungen
- Microsoft Defender für EndPoint Security
- Microsoft Edge

Jede der Basispläne wird regelmäßig aktualisiert und in inkrementellen Versionen veröffentlicht. In jeder Version werden Einstellungen zur vorherigen Version hinzugefügt und/oder entfernt, um sicherzustellen, dass der Basisplan den aktuellen Richtlinien entspricht. Über die Security Basisplan-Konsole in Endpoint Security können verschiedene Versionen verglichen werden, indem die Änderungen von Version zu Version sichtbar gemacht werden.

Anleitungen zum effektivsten Ändern der bereitgestellten Basisplan-Version finden Sie unter [Verwalten von Sicherheitsbasisplan-Profilen in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Nach der Bereitstellung eines Sicherheitsbasisplans können Sie den Bereitstellungsstatus überwachen und die Einstellungen geräteweise überprüfen.

Da die Sicherheitsbaselines viele Einstellungen enthalten, ist es wichtig, die Konfigurationsänderungen zu überprüfen und Tests durchzuführen, um sicherzustellen, dass alle Einstellungen für Ihre Geräte und Geschäftsanforderungen geeignet sind.

**Hinweis:** Es kann bis zu 24 Stunden dauern, bis die Berichtsdaten für Basispläne von der ersten Bereitstellung auf einem Gerät bis zu 6 Stunden für weitere Aktualisierungen angezeigt werden. 

Die häufigste Ursache dafür, dass eine Grundeinstellung nicht angewendet wird, ist, dass dieselbe Einstellung in einem anderen Profil verwendet wird. Dieses Szenario kann für ein bestimmtes Gerät untersucht werden, indem dieses Gerät im Knoten Gerätestatus des Security Basisplanprofils ausgewählt wird. Weitere Informationen finden Sie unter [Lösen von Konflikten für Sicherheitsbasispläne](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).