---
title: Offboarden von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 995ff59a8d7a869f27189cbeb0412bc576a422f6
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66342417"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboarden von Nicht-Windows-Geräten von Microsoft Defender Advanced Threat Protection (ATP)

Dazu gehen Sie so vor:

1. Folgen Sie der Dokumentation von Drittanbietern, um die Drittanbieterlösung von Microsoft Defender ATP zu trennen.
2. Entfernen Sie von Ihrem Azure Active Directory-Mandanten Berechtigungen für die Drittanbieterlösung:

    1. Melden Sie sich beim [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2125612) an.
    1. Wählen Sie **Alle Dienste** > **Azure Active Directory** > **Enterprise-Anwendungen** aus.
    1. Wählen Sie die Anwendung aus, die Sie offboarden möchten.
    1. Klicken Sie auf **Löschen**.

Weitere Informationen finden Sie unter [Offboard für Nicht-Windows-Geräte](https://go.microsoft.com/fwlink/?linkid=2143630).
