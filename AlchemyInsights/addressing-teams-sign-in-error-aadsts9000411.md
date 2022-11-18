---
title: Ansprechen von Teams-Anmeldefehler AADSTS9000411
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 02af6c9cbbfc97ccc1bb50c7c6ef205ff4246f3c
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66519024"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Ansprechen von Teams-Anmeldefehler AADSTS9000411

Wenn Sie sich bei Microsoft Teams anmelden, kann die Fehlermeldung angezeigt werden: **Es tut uns leid, aber wir haben Probleme, Sie in AADSTS9000411 anzumelden: Die Anforderung ist nicht richtig formatiert. Der Parameter "login_hint" ist doppelt vorhanden.**

Um dieses Problem zu beheben, stellen Sie bitte sicher, dass Ihre Microsoft Teams-Clients aktualisiert sind. Weitere Informationen zur Aktualisierung Ihres Clients finden Sie unter [Microsoft Teams aktualisieren](https://support.microsoft.com/office/update-microsoft-teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Wenn Sie Ihren Client aus irgendeinem Grund nicht aktualisieren können, werden durch das Abmelden des Clients die meisten zwischengespeicherten Daten gelöscht. Wenn Sie jedoch nach der Abmeldung/Anmeldung immer noch Probleme haben, beenden Sie Teams und löschen Sie bitte Ihren Clientcache, indem Sie die folgenden Schritte ausführen:
1. Microsoft Teams schließen.
2. Wechseln Sie zu: %appdata%\microsoft\teams, und löschen Sie alle Dateien.
3. Microsoft Teams erneut öffnen.
