---
title: Geräterückschreiben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: bdabcd57cfe6a856adba6bb221cb6f63f4c60f6f
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66518808"
---
# <a name="device-writeback"></a>Geräterückschreiben

Das Geräterückschreiben wird in den folgenden Szenarien verwendet:

- Aktivieren [Windows Hello for Business mithilfe der Hybridbereitstellung mit Zertifikatvertrauensstellung](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivieren des bedingten Zugriffs basierend auf Geräten für durch ADFS (2012 R2 oder höher) geschützte Anwendungen (Vertrauensstellungen vertrauender Parteien)

    **Hinweis**: Für das Geräterückschreiben ist ein Abonnement von Azure AD Premium erforderlich.

Dies bietet zusätzliche Sicherheit und Sicherheit, dass der Zugriff auf Anwendungen nur vertrauenswürdigen Geräten gewährt wird. Weitere Informationen zum bedingten Zugriff finden Sie unter [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).

Weitere Informationen zum Aktivieren des Geräterückschreibens für Geräte finden [Sie unter Aktivieren des Geräterückschreibens](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
