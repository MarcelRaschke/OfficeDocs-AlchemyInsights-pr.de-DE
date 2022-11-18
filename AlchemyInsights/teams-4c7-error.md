---
title: Teams 4c7-Fehler
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001211"
- "3472"
ms.openlocfilehash: 9e6427f104797ea191238cb039ccd495faca510d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66290683"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-Fehler in Microsoft Teams

Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert. Wenn Sie Active Directory-Verbunddienste (AD FS) (AD FS) bereitstellen, ist die Formularauthentifizierung für das Intranet standardmäßig nicht aktiviert. Wenn die integrierte Windows-Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mithilfe der Formularauthentifizierung anzumelden.

Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des MMC-Snap-Ins (AD FS Microsoft Management Console) auf dem Computer mit der lokalen Kopie von Active Directory. Gehen Sie dazu wie folgt vor: 

1. Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.
2. Wählen Sie unter **"Aktionen** " im Detailbereich " **Globale primäre Authentifizierung bearbeiten"** aus.
3. Wählen Sie auf der Registerkarte **"Intranet** " die Option **"Formularauthentifizierung**" aus.
4. Wählen Sie **"OK** " (oder **"Übernehmen") aus**.