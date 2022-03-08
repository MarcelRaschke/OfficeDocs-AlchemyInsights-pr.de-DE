---
title: Offboarding von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c97989c4b269461547e42376fb5fccf86fd593aa
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63161671"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboarding von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)

Dazu gehen Sie so vor:

1. Folgen Sie der Dokumentation des Drittanbieters, um die Verbindung zwischen der Drittanbieterlösung und Microsoft Defender ATP zu trennen.
2. Entfernen Sie aus Ihrem Azure Active Directory Mandanten Berechtigungen für die Drittanbieterlösung:

    1. Melden Sie sich beim [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2125612) an.
    1. Wählen Sie **"Alle Dienste** >  **Azure Active Directory** >  **Enterprise Anwendungen aus**.
    1. Wählen Sie die Anwendung aus, die Sie offboarden möchten.
    1. Klicken Sie auf **Löschen**.

Weitere Informationen finden Sie unter [Offboarding von Nicht-Windows-Geräten](https://go.microsoft.com/fwlink/?linkid=2143630).
