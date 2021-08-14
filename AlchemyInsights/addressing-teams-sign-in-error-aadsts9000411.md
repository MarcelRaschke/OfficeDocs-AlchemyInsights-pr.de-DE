---
title: Ansprechen von Teams-Anmeldefehler AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953022"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Ansprechen von Teams-Anmeldefehler AADSTS9000411

Wenn Sie sich bei Microsoft Teams anmelden, kann die Fehlermeldung angezeigt werden: **Es tut uns leid, aber wir haben Probleme, Sie in AADSTS9000411 anzumelden: Die Anforderung ist nicht richtig formatiert. Der Parameter "login_hint" ist doppelt vorhanden.**

Um dieses Problem zu beheben, stellen Sie bitte sicher, dass Ihre Microsoft Teams-Clients aktualisiert sind. Weitere Informationen zur Aktualisierung Ihres Clients finden Sie unter [Microsoft Teams aktualisieren](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Wenn Sie Ihren Client aus irgendeinem Grund nicht aktualisieren können, werden durch das Abmelden des Clients die meisten zwischengespeicherten Daten gelöscht. Wenn Sie jedoch nach der Abmeldung/Anmeldung immer noch Probleme haben, beenden Sie Teams und löschen Sie bitte Ihren Clientcache, indem Sie die folgenden Schritte ausführen:
1. Microsoft Teams schließen.
2. Wechseln Sie zu: %appdata%\microsoft\teams, und löschen Sie alle Dateien.
3. Microsoft Teams erneut öffnen.
