---
title: Dynamics 365 – Falsche Dashboard-Shows in Dynamics 365 Unified Interface
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: 'NOINDEX, NOFOLLOW'
localization_priority: Normal
ms.custom:
  - 1484
  - 6200024
---

# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Falsches Dashboard in der einheitlichen Dynamics 365-Schnittstelle

Es gibt mehrere Gründe, warum Sie möglicherweise ein anderes Dashboard sehen als das, das Sie erwarten:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Der Benutzer hat ein Benutzerstandarddashboard festgelegt. 

In der Regel können Sie festlegen, dass ein Benutzerstandarddashboard festgelegt ist, wenn die Schaltfläche **"Als Standard festlegen"** nicht in der Dashboard-Befehlsleiste angezeigt wird. Das Standarddashboard des Benutzers überschreibt alle anderen Standarddashboards, auch wenn sich das Standarddashboard des Benutzers nicht in der aktuellen App befindet.

Verwenden Sie die folgende Problemumgehung, um das Standarddashboard aufzuheben.

1. Erstellen Sie ein neues persönliches Dashboard.

2. Legen Sie dieses neue Dashboard als Benutzerstandard fest.

3. Löschen Sie dieses Dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Das Dashboard wird in der Sitemap festgelegt.

Möglicherweise haben Sie ein Standarddashboard der Organisation festgelegt, indem Sie ein Dashboard und unter "System anpassen" die Option "Als Standard festlegen" ausgewählt haben. Das im Sitemap-Designer definierte Dashboard hat jedoch Vorrang vor diesem Dashboard, wenn der Benutzer Darauf zugreifen kann.

Damit Benutzern das Dashboard angezeigt wird, das Sie als Standard für die Organisation festgelegt haben, können Sie die folgenden Aktionen ausführen:

* Festlegen dieses Dashboards in der Sitemap

* Entfernen des Zugriffs auf das von sitemap definierte Dashboard für diese Benutzer
