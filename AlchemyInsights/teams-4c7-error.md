---
title: Teams 4c7-Fehler
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
- "3472"
- "9001211"
ms.openlocfilehash: 6e1a1e72b69e9078141b9af8fddbdc120ce68ed9
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62631534"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-Fehler in Microsoft Teams

Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert. Wenn Sie Active Directory-Verbunddienste (AD FS) bereitstellen, ist die Formularauthentifizierung für das Intranet nicht standardmäßig aktiviert. Wenn Windows integrierte Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mithilfe der Formularauthentifizierung anzumelden.

Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des AD FS Microsoft Management Console (MMC)-Snap-Ins auf dem Computer mit der lokalen Kopie von Active Directory. Gehen Sie dazu wie folgt vor: 

1. Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.
2. Wählen Sie im Detailbereich unter **"Aktionen** " die Option **"Globale primäre Authentifizierung bearbeiten" aus**.
3. Wählen Sie auf der Registerkarte **"Intranet** " die Option **"Formularauthentifizierung" aus**.
4. Wählen Sie **"OK** " (oder **"Anwenden") aus**.