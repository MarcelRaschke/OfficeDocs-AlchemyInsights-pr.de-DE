---
title: Anwenden bewährter Methoden für abfragen der erweiterten Suche
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930132"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Anwenden bewährter Methoden für abfragen der erweiterten Suche

Wenden Sie die folgenden bewährten Methoden an, um schneller Ergebnisse zu erzielen und Timeouts beim Ausführen komplexer Abfragen zu vermeiden:

- Verwenden Sie beim Ausprobieren neuer Abfragen immer einen Grenzwert, um zu vermeiden, dass extrem große Resultsets abgerufen werden. Verwenden Sie dies auch, `count` um eine anfängliche Bewertung der Größe des Resultsets vorzunehmen.
- Verwenden Sie zunächst Zeitfilter. Im Idealfall beschränken Sie Ihre Abfragen auf sieben Tage.
- Fügen Sie am Anfang einer Abfrage direkt nach dem Zeitfilter die Filter hinzu, von denen erwartet wird, dass die meisten Daten entfernt werden.
- Wenn Sie nach vollständigen Token suchen, verwenden Sie den `has` Operator anstelle `contains` von .
- Führen Sie eine Suche für eine bestimmte Spalte und nicht für alle Spalten aus.
- Geben Sie beim Verknüpfen von Tabellen zuerst die Tabelle mit weniger Zeilen an.
- `project` nur die erforderlichen Spalten aus den Tabellen, die Sie verknüpft haben.

Weitere Informationen finden Sie unter ["Bewährte Methoden für erweiterte Suchabfragen".](https://go.microsoft.com/fwlink/?linkid=2144812)
