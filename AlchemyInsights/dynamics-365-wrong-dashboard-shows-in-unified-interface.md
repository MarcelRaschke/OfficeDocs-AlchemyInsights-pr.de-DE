---
title: Dynamics 365 – Falsches Dashboard in Dynamics 365 Unified Interface
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "6200024"
- "1484"
ms.openlocfilehash: 5756c10ded3a9d448e4e9cc3fb8a67fc4975d4fb
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66341422"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Falsches Dashboard in der einheitlichen Dynamics 365-Schnittstelle

Es gibt mehrere Gründe, warum möglicherweise ein anderes Dashboard angezeigt wird als das, das Sie erwarten:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Der Benutzer hat ein Benutzerstandarddashboard festgelegt. 

In der Regel können Sie feststellen, dass ein Benutzerstandarddashboard festgelegt ist, wenn die Schaltfläche " **Als Standard festlegen** " nicht in der Befehlsleiste des Dashboards angezeigt wird. Das Standarddashboard des Benutzers überschreibt alle anderen Standarddashboards, auch wenn sich das Standarddashboard des Benutzers nicht in der aktuellen App befindet.

Verwenden Sie die folgende Problemumgehung, um das Standarddashboard aufzugeben.

1. Erstellen Sie ein neues persönliches Dashboard.

2. Legen Sie das neue Dashboard als Benutzerstandard fest.

3. Löschen Sie dieses Dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Das Dashboard wird in der Sitemap festgelegt.

Möglicherweise haben Sie ein Standarddashboard der Organisation festgelegt, indem Sie ein Dashboard auswählen und unter "System anpassen" die Option "Als Standard festlegen" auswählen. Das im Sitemap-Designer definierte Dashboard hat jedoch Vorrang vor diesem Dashboard, wenn der Benutzer Zugriff darauf hat.

Damit Benutzern das Dashboard angezeigt wird, das Sie als Standard für die Organisation festgelegt haben, haben Sie folgende Möglichkeiten:

* Festlegen dieses Dashboards in der Sitemap

* Entfernen des Zugriffs auf das von der Sitemap definierte Dashboard für diese Benutzer
