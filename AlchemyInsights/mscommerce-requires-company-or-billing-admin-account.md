---
title: Herstellen einer Verbindung mit dem MSCommerce-Modul
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 81487107f0a4a7c3b16fcdf522af08552b6f74ce
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66351039"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce erfordert ein Firmen- oder Abrechnungsadministratorkonto

Das MSCommerce-Modul erfordert ein Konto mit Unternehmens- oder Abrechnungsadministratorberechtigungen. Wenn Sie den folgenden Fehler erhalten, müssen Sie erneut eine Verbindung mit einem anderen Konto herstellen.

*ErrorMessage – Der Remoteserver hat einen Fehler zurückgegeben: (403) Verboten. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Fehler beim Wiederholen ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Wenn Ihr Konto nicht über die Berechtigungen "Unternehmensadministrator" oder "Abrechnungsadministrator" verfügt, wenden Sie sich an Ihre IT-Admin.
