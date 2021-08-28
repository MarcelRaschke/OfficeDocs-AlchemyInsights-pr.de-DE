---
title: Aktivieren von Teams-Webinaren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5efb8ffad0ad2c7d32a2ac334b960484b6fa5545
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325340"
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

**Hinweis**: Wenn die anonyme Teilnahme in den Besprechungseinstellungen deaktiviert ist, können anonyme Benutzer nicht an Webinaren teilnehmen. Weitere Informationen zum Aktivieren dieser Einstellung finden Sie unter  [Verwalten von Besprechungseinstellungen in Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-settings-in-teams). 

Weitere Informationen zum Konfigurieren, wer sich für Webinare registrieren kann, und zum Verwalten dieser Richtlinien mithilfe von Teams PowerShell finden Sie unter [Konfigurieren, wer sich für Webinare registrieren kann](https://docs.microsoft.com/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Weitere Informationen zu den Einstellungen für Microsoft Listen finden Sie unter  [Steuerelementeinstellungen für Microsoft Listen](https://docs.microsoft.com/sharepoint/control-lists). 