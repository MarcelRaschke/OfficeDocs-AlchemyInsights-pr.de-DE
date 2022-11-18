---
title: Beheben von Transportregeln
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
ms.openlocfilehash: 24628d69ae6f26e87f6f4906698184573ec4d033
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66380289"
---
# <a name="fix-transport-rules"></a>Beheben von Transportregeln

Eine benutzerdefinierte Nachrichtenflussregel wirkte sich auf diese Nachricht aus. Gehen Sie wie folgt vor, um die genaue Regel zu überprüfen:

1. Notieren Sie sich in den Übermittlungsergebnissen unter **"Zusätzliche Informationen**" die **GUID** oder den **Richtliniennamen**.
2. Starten Sie die Exchange-Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Führen Sie diesen Befehl aus (mithilfe der GUID aus Ihrer Übermittlung):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Überprüfen Sie die Beschreibung, um die konfigurierten Bedingungen anzuzeigen, die sich auf die Nachricht auswirkten.

Weitere Informationen finden Sie unter [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
