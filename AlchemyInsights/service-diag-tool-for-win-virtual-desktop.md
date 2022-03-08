---
title: Dienstdiagnosetool für Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c13798d03f2bab1dd46665b6d95241aae276ab3b
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63084934"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Dienstdiagnosetool für Windows Virtual Desktop

Windows Virtual Desktop (WVD) bietet ein Diagnosetool, mit dem Administratoren Fehler über eine einzelne Schnittstelle erkennen können. Dieses Tool protokolliert diagnosebezogene Informationen immer dann, wenn WVD von einer Person verwendet wird, der eine WVD-Rolle zugewiesen wurde. Jedes Protokoll enthält Informationen zur WVD-Rolle, die an der Aktivität beteiligt ist, die Fehlermeldungen, die während der Sitzung angezeigt werden, und die Informationen zum Mandanten und Benutzer. Azure Log Analytics kann so konfiguriert werden, dass das vom Diagnosetool erstellte Aktivitätsprotokoll erfasst wird. Dazu gehen Sie so vor:

1. Erstellen eines Protokollanalysearbeitsbereichs mit dem [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) oder über [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Verbinden von Windows-Computern mit Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Sie erhalten die Arbeitsbereichs-ID und den Primärschlüssel Ihres Arbeitsbereichs. Der Setup-Assistent benötigt diese Informationen, um den Agent ordnungsgemäß zu konfigurieren und um sicherzustellen, dass er mit Azure Monitor kommunizieren kann.
1. [Diagnosedaten in den Arbeitsbereich übertragen](https://go.microsoft.com/fwlink/?linkid=2128284). Sie können Diagnosedaten aus dem WVD-Mandanten in Log Analytics für Ihren Arbeitsbereich übertragen.
1. [Identifizieren und Diagnostizieren von Internen](https://go.microsoft.com/fwlink/?linkid=2128338) oder externen Problemen in Bezug auf WVD.

Weitere Informationen zum Konfigurieren des Dienstdiagnosetools für WVD finden Sie unter [Verwenden der Protokollanalyse für das Diagnosefeature](https://go.microsoft.com/fwlink/?linkid=2128084).
