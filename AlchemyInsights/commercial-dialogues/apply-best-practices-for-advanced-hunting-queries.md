---
title: Anwenden bewährter Methoden für erweiterte Suchabfragen
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
ms.openlocfilehash: 4fa262a3f4c3d818bce7f282def90ec2591fc9ce
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66369651"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Anwenden bewährter Methoden für erweiterte Suchabfragen

Wenden Sie die folgenden bewährten Methoden an, um Ergebnisse schneller zu erhalten und Timeouts beim Ausführen komplexer Abfragen zu vermeiden:

- Verwenden Sie beim Versuch neuer Abfragen immer einen Grenzwert, um zu vermeiden, dass extrem große Resultsets angezeigt werden. Verwenden Sie `count` außerdem eine erste Bewertung der Größe des Resultsets.
- Verwenden Sie als erstes Zeitfilter. Im Idealfall beschränken Sie Ihre Abfragen auf sieben Tage.
- Fügen Sie am Anfang einer Abfrage direkt nach dem Zeitfilter die Filter hinzu, von der erwartet wird, dass die meisten Daten entfernt werden.
- Wenn Sie nach vollständigen Token suchen, verwenden Sie den `has` Operator anstelle von `contains`.
- Führen Sie eine Suche für eine bestimmte Spalte statt für alle Spalten aus.
- Geben Sie beim Verknüpfen von Tabellen zuerst die Tabelle mit weniger Zeilen an.
- `project` nur die erforderlichen Spalten aus den Tabellen, die Sie verknüpft haben.

Weitere Informationen finden Sie unter [Bewährte Methoden für Abfragen zur erweiterten Suche](https://go.microsoft.com/fwlink/?linkid=2144812).
