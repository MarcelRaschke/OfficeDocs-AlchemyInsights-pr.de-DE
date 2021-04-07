---
title: Identifizieren von Problemen mit Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590295"
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
