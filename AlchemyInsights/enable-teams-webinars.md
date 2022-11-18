---
title: Aktivieren von Teams-Webinaren
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9006672"
- "11513"
ms.date: 06/02/2021
ms.openlocfilehash: 6f663c39b728f724642015e68aa30573a213b557
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66339393"
---
# <a name="enable-teams-webinars"></a>Aktivieren von Teams-Webinaren

Die Webinarregistrierung ist standardmäßig aktiviert. Wenn Sie die Besprechungsregistrierung deaktivieren möchten, können Sie das Microsoft Teams Admin Center verwenden: 

1. Navigieren Sie zum [Teams Admin Center](https://admin.teams.microsoft.com/policies/meetings). 

2. Wählen Sie die **Globale Richtlinie (organisationsweiter Standard)** oder eine andere spezifische Richtlinie aus. 

3. Legen Sie unter **Allgemein** die Option **Besprechungsregistrierung zulassen** auf **Aus** fest. 

Wenn die Besprechungsregistrierung auf **Ein** festgelegt ist, können Sie auch über das Microsoft Teams Admin Center verwalten, wer sich für Microsoft Teams-Webinare registriert: 

1. Navigieren Sie zum [Teams Admin Center](https://admin.teams.microsoft.com/policies/meetings). 

2. Wählen Sie die **Globale Richtlinie (organisationsweiter Standard)** oder eine andere spezifische Richtlinie aus. 

3. Navigieren Sie unter **Allgemein** zur Einstellung **Wer kann sich registrieren**, und wählen Sie entweder **Alle** oder **Alle im Unternehmen** aus. 

**Hinweis**: Wenn die anonyme Teilnahme in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen. Weitere Informationen zum Aktivieren dieser Einstellung finden Sie unter [Verwalten von Besprechungseinstellungen in Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-settings-in-teams). 

Weitere Informationen zum Konfigurieren der Personen, die sich für Webinare anmelden können, und zum Verwalten dieser Richtlinien mit Teams PowerShell finden Sie unter [Konfigurieren der Personen, die sich für Webinare anmelden können](https://docs.microsoft.com/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter [Steuern der Einstellungen für Microsoft Listen](https://docs.microsoft.com/sharepoint/control-lists). 