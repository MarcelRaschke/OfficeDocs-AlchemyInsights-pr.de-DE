---
title: Fehlercode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Wenn beim Aktivieren von Office 2013 für Remotedesktopdienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung in Betracht ziehen.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316685"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fehler bei der Aktivierung Office 2013 für Remotedesktopdienste

Wenn beim Aktivieren von Office 2013 für Remotedesktopdienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung in Betracht ziehen.
  
|**Registrierungsschlüssel**|**Type**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows Geräten.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Hinweis:** ADAL ist in Microsoft 365 Apps for Enterprise und Office 2016 standardmäßig aktiviert. Remotedesktopdienste (RDS) wurde zuvor als Terminaldienste bezeichnet.
  