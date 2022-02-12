---
title: Geräterückschreiben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: 418579800b4ee66e99d704ca1d516f3258ff4df3
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62555571"
---
# <a name="device-writeback"></a>Geräterückschreiben

Das Geräterückschreiben wird in den folgenden Szenarien verwendet:

- Aktivieren [von Windows Hello for Business mithilfe einer hybriden Bereitstellung mit Zertifikatvertrauensstellung](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivieren des bedingten Zugriffs basierend auf Geräten für ADFS (2012 R2 oder höher) geschützte Anwendungen (Vertrauensstellungen der vertrauenden Seite)

    **Hinweis**: Für das Geräterückschreiben ist ein Abonnement für Azure AD Premium erforderlich.

Dies bietet zusätzliche Sicherheit und Sicherheit, dass der Zugriff auf Anwendungen nur vertrauenswürdigen Geräten gewährt wird. Weitere Informationen zum bedingten Zugriff finden Sie unter [Verwalten von Risiken mit bedingtem Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) und [Einrichten des lokalen bedingten Zugriffs mit Azure Active Directory Geräteregistrierung](https://docs.microsoft.com/azure/active-directory/devices/overview).

Weitere Informationen zum Aktivieren des Geräterückschreibens für Geräte finden Sie unter [Aktivieren des Geräterückschreibens](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
