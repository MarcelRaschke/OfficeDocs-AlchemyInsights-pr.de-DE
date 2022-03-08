---
title: Verbinden zum MSModule-Modul
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 5d5a7ba73dc8e56f33a9b3586b4d231c94b59b45
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63225141"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MS Commerce erfordert ein Konto des Unternehmens oder des Abrechnungsadministrators

Das MSModule erfordert ein Konto mit Den Berechtigungen "Unternehmen" oder "Abrechnungsadministrator". Wenn der folgende Fehler angezeigt wird, müssen Sie die Verbindung mit einem anderen Konto wiederherstellen.

*ErrorMessage : Der Remoteserver hat einen Fehler zurückgegeben: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MS Dropdown\1.2\MS Connectors.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Fehler beim Wiederholen ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Wenn Ihr Konto nicht über Berechtigungen für den Unternehmens- oder Abrechnungsadministrator verfügt, wenden Sie sich an Ihren IT-Administrator.
