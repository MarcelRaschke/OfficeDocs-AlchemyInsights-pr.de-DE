---
title: Offboarding von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c90a0e6bc779cc9112f9b8ad3e87fbfb22fb6a7c
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62687912"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboarding von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)

Dazu gehen Sie so vor:

1. Folgen Sie der Dokumentation des Drittanbieters, um die Verbindung zwischen der Drittanbieterlösung und Microsoft Defender ATP zu trennen.
2. Entfernen Sie aus Ihrem Azure Active Directory Mandanten Berechtigungen für die Drittanbieterlösung:

    1. Melden Sie sich beim [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2125612) an.
    1. Wählen Sie **"Alle Dienste** >  **Azure Active Directory** >  **Enterprise Anwendungen aus**.
    1. Wählen Sie die Anwendung aus, die Sie offboarden möchten.
    1. Wählen Sie **Löschen** aus.

Weitere Informationen finden Sie unter [Offboarding von Nicht-Windows-Geräten](https://go.microsoft.com/fwlink/?linkid=2143630).
