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
ms.openlocfilehash: e6152f536ad524894755f031d1e2740e5fc63430
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62624964"
---
# <a name="fix-transport-rules"></a>Beheben von Transportregeln

Diese Nachricht wurde von einer benutzerdefinierten Nachrichtenflussregel beeinflusst. Gehen Sie folgendermaßen vor, um die genaue Regel zu überprüfen:

1. Notieren Sie in den Übermittlungsergebnissen unter **zusätzlichen Informationen** die **GUID** oder den **Richtliniennamen**.
2. Starten Sie Exchange Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Führen Sie diesen Befehl aus (mithilfe der GUID aus Ihrer Übermittlung):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Überprüfen Sie die Beschreibung, um die konfigurierten Bedingungen anzuzeigen, die sich auf die Nachricht auswirkten.

Weitere Informationen finden Sie unter ["Get-TransportRule"](https://go.microsoft.com/fwlink/?linkid=2101523).
