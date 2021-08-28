---
title: Verbinden zum MSModule-Modul
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974668"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MS Commerce erfordert ein Konto des Unternehmens oder des Abrechnungsadministrators

Das MSModule erfordert ein Konto mit Den Berechtigungen "Unternehmen" oder "Abrechnungsadministrator". Wenn der folgende Fehler angezeigt wird, müssen Sie die Verbindung mit einem anderen Konto wiederherstellen.

*ErrorMessage : Der Remoteserver hat einen Fehler zurückgegeben: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MS Dropdown\1.2\MS Connectors.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Fehler beim Wiederholen ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Wenn Ihr Konto nicht über Berechtigungen für den Unternehmens- oder Abrechnungsadministrator verfügt, wenden Sie sich an Ihren IT-Administrator.
