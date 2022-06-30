---
title: Diagnose für verschiedene Probleme beim Zugriff auf Ports
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9005220"
- "9035"
ms.date: 03/19/2021
ms.openlocfilehash: b7699816c9818e84fba328e2334b4d542dac4a56
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66511824"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnose für verschiedene Probleme beim Zugriff auf Ports

Führen Sie die folgenden Schritte aus, um die verschiedenen Probleme beim Portzugriff zu beheben:

1. Beenden/Freigabe der virtuellen Maschine (VM) vom Portal aus, starten Sie die VM neu und testen Sie diese erneut. 
2. Überprüfen Sie die Netzwerkeinstellungen Ihrer VM, um festzustellen, ob Network Security Groups (NSGs) den Datenverkehr blockieren. Sie können auch das [IP-Flussüberprüfungstool von Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) verwenden, um zu überprüfen, ob NSGs den Datenverkehr blockieren, benutzerdefinierte Routen (User Defined Routes, UDRs), die Ihren Datenverkehr zurück zu lokalen ('Standardroute' 0.0.0.0/0) oder zu einer Netzwerk-Anwendung umleiten.
Wenn nach dem Ausführen der obigen Schritte weiterhin Probleme auftreten, geben Sie den VM-Namen und den TCP-Port an, an den Sie E-Mails zur weiteren Diagnose senden möchten.

**Empfohlene Dokumente**

[Einschränkungen und Empfehlungen für das Senden ausgehender E-Mails über Port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)