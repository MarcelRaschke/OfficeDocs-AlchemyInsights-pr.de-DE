---
title: Fehlercode 0x15
author: cmcatee-MSFT
ms.author: cmcatee
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "2000022"
- "919"
ms.date: 04/21/2020
ms.openlocfilehash: bac42fb451bd40fd246ab0eff2fda549b15abdb4
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63129269"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fehler bei der Aktivierung Office 2013 für Remotedesktopdienste

Wenn beim Aktivieren von Office 2013 für RDS-Bereitstellungen (RemoteDesktopdienste) ein Fehler angezeigt wird, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung in Betracht ziehen.
  
|**Registrierungsschlüssel**|**Typ**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows Geräten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
**Hinweis**: ADAL ist in Microsoft 365 Apps for Enterprise und Office 2016 standardmäßig aktiviert. Remotedesktopdienste (RDS) wurde zuvor als Terminaldienste bezeichnet.
  