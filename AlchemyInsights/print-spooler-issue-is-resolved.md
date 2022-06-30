---
title: Druckerspoolerproblem wurde behoben
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9002659"
- "5151"
ms.date: 07/8/2020
ms.openlocfilehash: 402e9845f54389bd611c6144f1895ff865baad8e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66400647"
---
# <a name="print-spooler-issue-is-resolved"></a>Druckerspoolerproblem wurde behoben

Wenn Ihr Gerät mit Windows 10 **OS Build 19041.329** aktualisiert wurde, kann es bei bestimmten Druckern zu einem Problem gekommen sein. Der Druckerspooler löste beim Versuch zu drucken möglicherweise einen Fehler aus oder wurde unerwartet beendet, und es wurde vom betroffenen Drucker keine Ausgabe gedruckt. Dieses Problem wurde in Betriebssystembuild **19041.331** behoben ([KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)).  

**Untersuchung läuft**

Die LSASS-Datei (Local Security Authority Subsystem Service), **Isass.exe**, schlägt auf einigen Geräten mit der Fehlermeldung "Fehler bei einem kritischen Systemprozess, C:\WINDOWS\system32\Isass.exe, mit Statuscode c0000008. Der Computer muss jetzt neu gestartet werden" fehl.  **Microsoft arbeitet an einer Lösung und stellt in einer kommenden Version ein Update bereit.**

Weitere Informationen finden Sie unter [Bekannte Probleme in Windows 10 Version 2004](https://docs.microsoft.com/windows/release-health/resolved-issues-windows-10-20h2).