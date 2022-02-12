---
title: Active Directory wird nicht synchronisiert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 27b68d147e7ed20d5ea84828abe02196372483ae
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62563023"
---
# <a name="active-directory-not-syncing"></a>Active Directory wird nicht synchronisiert

Wenn Sie Synchronisierungsfehler erhalten, z. B. "keine kürzliche Synchronisierung", oder beachten Sie, dass der Status der Verzeichnissynchronisierung im Office Verwaltungsportal besagt: "Letzte Synchronisierung vor mehr als 3 Tagen", kann es sein, dass AADConnect über falsche Einstellungen oder unzureichende Berechtigungen zum Ausführen einer Synchronisierung verfügt.  

Durch erneutes Installieren von AADConnect mithilfe von Expresseinstellungen kann das Problem schnell behoben werden:

1. [Laden Sie die neueste Version von AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771) herunter.

2. [Folgen Sie den Anweisungen für die Expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect muss unter Windows Server 2012 oder höher installiert sein. Dieser Server muss der Domäne beigetreten sein und kann ein Domänencontroller oder ein Mitgliedsserver sein. Eine vollständige Liste der Azure AD Verbinden Anforderungen und Voraussetzungen erhalten Sie unter ["Voraussetzungen für Azure AD Verbinden](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)".

Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Konten und Berechtigungen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
