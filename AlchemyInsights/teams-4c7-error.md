---
title: Teams 4c7-Fehler
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
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049307"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-Fehler in Microsoft Teams

Dieser Fehler tritt auf, da Microsoft Teams die Formularauthentifizierung erfordert. Wenn Sie Active Directory-Verbunddienste (AD FS) bereitstellen, ist die Formularauthentifizierung für das Intranet nicht standardmäßig aktiviert. Wenn Windows integrierte Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mithilfe der Formularauthentifizierung anzumelden.

Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des AD FS Microsoft Management Console (MMC)-Snap-Ins auf dem Computer mit der lokalen Kopie von Active Directory. Gehen Sie dazu wie folgt vor: 

1. Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien.**
2. Wählen Sie im Detailbereich unter **Aktionen** die Option **"Globale primäre Authentifizierung bearbeiten"** aus.
3. Wählen Sie auf der Registerkarte **"Intranet"** die Option **"Formularauthentifizierung" aus.**
4. Wählen Sie **"OK"** (oder **"Anwenden")** aus.