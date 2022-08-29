---
title: Identifizieren von Problemen mit Windows Virtual Desktop
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
- "10871"
- "10874"
ms.date: 04/5/2021
ms.openlocfilehash: d5137ece9207ce191044577749ae3f70c05da594
ms.sourcegitcommit: c524d66c406fcb7c0de677d2aa465e04e4f5553a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/16/2022
ms.locfileid: "67358375"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identifizieren von Problemen mit Windows Virtual Desktop

Windows Virtual Desktop-Diagnose verwendet nur ein PowerShell-Cmdlet, enthält aber viele optionale Parameter, um Probleme einzugrenzen und zu isolieren. Erste Schritte: 

1. Laden Sie das Windows Virtual Desktop PowerShell-Modul herunter, und importieren Sie es. Weitere Informationen finden Sie unter [Windows Virtual Desktop-Cmdlets für Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Führen Sie das folgende Cmdlet aus, um sich bei Ihrem Konto anmelden:
    
    Beispiel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**HINWEIS:** Alle Abfragen mit PowerShell müssen entweder die Parameter "-UserName" oder "-ActivityID" enthalten. Informationen zu den Überwachungsfunktionen finden Sie unter [Protokollanalyse für die Diagnosefunktion](https://go.microsoft.com/fwlink/?linkid=2126847).

Führen Sie das folgende Cmdlet aus, um Diagnoseaktivitäten nach Benutzer zu filtern:

Beispiel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Es gibt eine Liste von Filtern, die Sie ausführen können, um Probleme zu diagnostizieren. Weitere Informationen zur Diagnose von Problemen finden Sie unter [Ermitteln und Diagnostizieren von Problemen mit Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Weitere Informationen zu üblichen Fehlern finden Sie unter [Häufig auftretende Fehlerszenarien](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
