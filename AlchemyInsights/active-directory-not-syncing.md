---
title: Active Directory wird nicht synchronisiert
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 97eacfb5ae9237f6a7d62fb44aa915589a662831
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66313743"
---
# <a name="active-directory-not-syncing"></a>Active Directory wird nicht synchronisiert

Wenn Sie Synchronisierungsfehler wie "keine kürzliche Synchronisierung" erhalten oder feststellen, dass der Verzeichnissynchronisierungsstatus im Office-Verwaltungsportal "Letzte Synchronisierung vor mehr als 3 Tagen" lautet, kann es sein, dass AADConnect falsche Einstellungen oder unzureichende Berechtigungen zum Ausführen einer Synchronisierung hat.  

Durch erneutes Installieren von AADConnect mithilfe von Expresseinstellungen kann das Problem schnell behoben werden:

1. [Laden Sie die neueste Version von AADConnect herunter](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Befolgen Sie die Anweisungen für die Expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect muss unter Windows Server 2012 oder höher installiert sein. Dieser Server muss der Domäne beigetreten sein und kann ein Domänencontroller oder ein Mitgliedsserver sein. Eine vollständige Liste der Azure AD Connect-Anforderungen und -Voraussetzungen erfahren Sie unter ["Voraussetzungen für Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)".

Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Konten und Berechtigungen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
