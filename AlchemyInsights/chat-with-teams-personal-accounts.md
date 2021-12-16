---
title: Chatten mit Benutzern mit Teams persönlichen Konten
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
- "9000738"
- "16099"
ms.openlocfilehash: 3a4ce34ae3a4a1fc9af9fb2308aebad4f722a7cc
ms.sourcegitcommit: 6da5cdc3a5a109fa7db08374db61c8bc047e3eb4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/16/2021
ms.locfileid: "61548712"
---
# <a name="chat-with-users-with-teams-personal-accounts"></a>Chatten mit Benutzern mit Teams persönlichen Konten

Die Kommunikation mit Benutzern, deren Konten nicht von einer Organisation verwaltet werden (persönliche Konten), ist standardmäßig auf **"Ein"** festgelegt. Administratoren können diese Einstellung für die Organisation aktivieren oder deaktivieren, um zu steuern, ob Benutzer Nachrichten von persönlichen Konten senden oder empfangen können.

1. Wechseln Sie im Teams Admin Center zur Seite  >  [**"Externer Zugriff für**](https://admin.teams.microsoft.com/company-wide-settings/external-communications) Benutzer".
2. Wählen Sie im Abschnitt Teams Konto, das **nicht von einem Organisationsabschnitt verwaltet wird,** den Umschalter aus, um die Einstellung zu deaktivieren oder zu aktivieren.

Weitere Informationen finden Sie unter [Blockieren unerwünschter Kontakte mit externen nicht verwalteten Teams Benutzern.](https://docs.microsoft.com/microsoftteams/manage-external-access#block-unsolicited-contact-with-external-unmanaged-teams-users)

Sie können diese Einstellung auch mithilfe von PowerShell verwalten. Einstellungen sind: 

- `CsTenantFederationConfiguration [-AllowTeamsConsumer <Boolean>]` und `[AllowTeamsConsumerInbound]`
- Auf Benutzerebene `CsExternalAccessPolicy [-EnableTeamsConsumerAccess <Boolean>]` und `[-EnableTeamsConsumerInbound <Boolean>]`

Weitere Informationen finden Sie im Referenzhandbuch für [Set-CsTenantFederationConfiguration](https://docs.microsoft.com/powershell/module/skype/set-cstenantfederationconfiguration?view=skype-ps&preserve-view=true).
