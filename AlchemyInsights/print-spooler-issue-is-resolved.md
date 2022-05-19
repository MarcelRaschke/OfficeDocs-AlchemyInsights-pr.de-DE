---
title: Druckerspoolerproblem wurde behoben
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 1a5794c127dd0262b7a5fe565879353a09e118f3
ms.sourcegitcommit: c2b6eee90fbce71e65b4f7e95979344d875adc61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2022
ms.locfileid: "65593840"
---
# <a name="print-spooler-issue-is-resolved"></a>Druckerspoolerproblem wurde behoben

Wenn Ihr Gerät mit Windows 10 **OS Build 19041.329** aktualisiert wurde, kann es bei bestimmten Druckern zu einem Problem gekommen sein. Der Druckerspooler löste beim Versuch zu drucken möglicherweise einen Fehler aus oder wurde unerwartet beendet, und es wurde vom betroffenen Drucker keine Ausgabe gedruckt. Dieses Problem wurde in Betriebssystembuild **19041.331** behoben ([KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)).  

**Untersuchung läuft**

Die LSASS-Datei (Local Security Authority Subsystem Service), **Isass.exe**, schlägt auf einigen Geräten mit der Fehlermeldung "Fehler bei einem kritischen Systemprozess, C:\WINDOWS\system32\Isass.exe, mit Statuscode c0000008. Der Computer muss jetzt neu gestartet werden" fehl.  **Microsoft arbeitet an einer Lösung und stellt in einer kommenden Version ein Update bereit.**

Weitere Informationen finden Sie unter [Bekannte Probleme in Windows 10 Version 2004](https://docs.microsoft.com/windows/release-health/resolved-issues-windows-10-20h2).