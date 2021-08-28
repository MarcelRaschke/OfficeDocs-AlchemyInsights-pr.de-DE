---
title: Beheben von Transportregeln
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034753"
---
# <a name="fix-transport-rules"></a>Beheben von Transportregeln

Diese Nachricht wurde von einer benutzerdefinierten Nachrichtenflussregel beeinflusst. Gehen Sie folgendermaßen vor, um die genaue Regel zu überprüfen:

1. Notieren Sie sich in den Übermittlungsergebnissen unter **"Zusätzliche Informationen"** die **GUID** oder den **Richtliniennamen.**
2. Starten Sie Exchange Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Führen Sie diesen Befehl aus (mithilfe der GUID aus Ihrer Übermittlung):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Überprüfen Sie die Beschreibung, um die konfigurierten Bedingungen anzuzeigen, die sich auf die Nachricht auswirkten.

Weitere Informationen finden Sie unter [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
