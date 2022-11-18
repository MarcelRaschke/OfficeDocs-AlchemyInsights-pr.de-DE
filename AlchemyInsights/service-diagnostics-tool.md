---
title: Dienstdiagnosetool für Windows Virtual Desktop
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9004219"
- "10873"
ms.date: 04/5/2021
ms.openlocfilehash: 09c837a4c48315a5d0045f0fa6ff0f9ffb4556cf
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66316960"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Dienstdiagnosetool für Windows Virtual Desktop

Windows Virtual Desktop (WVD) bietet ein Diagnosetool, mit dem Administratoren Fehler über eine einzelne Schnittstelle erkennen können. Dieses Tool protokolliert diagnosebezogene Informationen immer dann, wenn WVD von einer Person verwendet wird, der eine WVD-Rolle zugewiesen wurde. Jedes Protokoll enthält Informationen zur WVD-Rolle, die an der Aktivität beteiligt ist, die Fehlermeldungen, die während der Sitzung angezeigt werden, und die Informationen zum Mandanten und Benutzer. Mit den folgenden Schritten kann Azure Log Analytics so konfiguriert werden, dass das vom Diagnosetool erstellte Aktivitätsprotokoll erfasst wird:

1. Erstellen eines Protokollanalysearbeitsbereichs mit dem [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) oder über [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Verbinden von Windows-Computern mit Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Sie erhalten die Arbeitsbereichs-ID und den Primärschlüssel Ihres Arbeitsbereichs. Der Setup-Assistent benötigt diese Informationen, um den Agent ordnungsgemäß zu konfigurieren und um sicherzustellen, dass er mit Azure Monitor kommunizieren kann.

1. [Diagnosedaten in den Arbeitsbereich übertragen](https://go.microsoft.com/fwlink/?linkid=2128284). Sie können Diagnosedaten aus dem WVD-Mandanten in Log Analytics für Ihren Arbeitsbereich übertragen.

1. [Identifizieren und Diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) von Problemen, die in Bezug auf WVD intern oder extern sind.

Weitere Informationen zum Konfigurieren des Dienstdiagnosetools für WVD finden Sie unter „Verwenden von Log Analytics für die Diagnosefunktion“.