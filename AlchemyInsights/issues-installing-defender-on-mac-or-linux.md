---
title: Probleme beim Installieren von Microsoft Defender auf Mac oder unter Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898607"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Probleme beim Installieren von Microsoft Defender auf Mac oder unter Linux

**Mac**

- Stellen Sie sicher, dass die Systemanforderungen erfüllt sind, bevor Sie Microsoft Defender ATP für Mac installieren. Weitere Informationen finden Sie unter [Installieren von Microsoft Defender ATP für Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Lesen Sie die Informationen in der Datei „/Library/Logs/Microsoft/mdatp/install.log“.

**Linux**

- Stellen Sie sicher, dass die Systemanforderungen erfüllt sind, bevor Sie Microsoft Defender ATP für Linux installieren. Weitere Informationen finden Sie unter [Installieren von MDATP für Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Um zu überprüfen, ob der MDATP-Dienst ausgeführt wird, lesen Sie [Fehler bei der Installation](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Informationen zur Problembehandlung und zum Beheben von Fehlern, wenn der Dienst nicht ausgeführt wird, finden Sie unter [Schritte zur Problembehandlung, wenn der MDATP-Dienst nicht ausgeführt wird](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Schritte zum Überprüfen der Clientkonfiguration, um den Zustand des Produkts zu überprüfen, und zum Ausführen eines Erkennungstests für die EICAR-Textdatei finden Sie unter [Clientkonfiguration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Hinweis** Eine Liste der unterstützten Dateisysteme für zugriffsbasierte Aktivitäten finden Sie unter [Microsoft Defender ATP für Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).