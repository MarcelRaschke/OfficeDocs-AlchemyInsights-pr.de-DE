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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967800"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboarding von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)

Dazu gehen Sie so vor:

1. Folgen Sie der Dokumentation des Drittanbieters, um die Verbindung zwischen der Drittanbieterlösung und Microsoft Defender ATP zu trennen.
2. Entfernen Sie aus Ihrem Azure Active Directory Mandanten Berechtigungen für die Drittanbieterlösung:

    1. Melden Sie sich beim [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2125612) an.
    1. Wählen Sie **alle Dienste**  >  **Azure Active Directory**  >  **Enterprise Anwendungen** aus.
    1. Wählen Sie die Anwendung aus, die Sie offboarden möchten.
    1. Wählen Sie **Löschen** aus.

Weitere Informationen finden Sie unter [Offboarding von Nicht-Windows-Geräten.](https://go.microsoft.com/fwlink/?linkid=2143630)
