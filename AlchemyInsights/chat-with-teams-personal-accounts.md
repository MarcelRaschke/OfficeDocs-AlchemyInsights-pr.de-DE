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
ms.openlocfilehash: 46afc631c1f019d34563428c36a4f5d9abbdc196
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62657130"
---
# <a name="chat-with-users-with-teams-personal-accounts"></a>Chatten mit Benutzern mit Teams persönlichen Konten

Die Kommunikation mit Benutzern, deren Konten nicht von einer Organisation verwaltet werden (persönliche Konten), ist standardmäßig auf **"Ein** " festgelegt. Administratoren können diese Einstellung für die Organisation aktivieren oder deaktivieren, um zu steuern, ob Benutzer Nachrichten von persönlichen Konten senden oder empfangen können.

1. Wechseln Sie im Teams Admin Center zur Seite "[**UsersExternal**](https://admin.teams.microsoft.com/company-wide-settings/external-communications)  >  Access".
2. Wählen Sie im Abschnitt **Teams Konto, das nicht von einem Organisationsabschnitt verwaltet wird**, den Umschalter aus, um die Einstellung zu deaktivieren oder zu aktivieren.

Weitere Informationen finden Sie unter [Blockieren unerwünschter Kontakte mit externen nicht verwalteten Teams Benutzern](https://docs.microsoft.com/microsoftteams/manage-external-access#block-unsolicited-contact-with-external-unmanaged-teams-users).

Sie können diese Einstellung auch mithilfe von PowerShell verwalten. Einstellungen sind: 

- `CsTenantFederationConfiguration [-AllowTeamsConsumer <Boolean>]` und `[AllowTeamsConsumerInbound]`
- Auf Benutzerebene `CsExternalAccessPolicy [-EnableTeamsConsumerAccess <Boolean>]` und `[-EnableTeamsConsumerInbound <Boolean>]`

Weitere Informationen finden Sie im Referenzhandbuch für [Set-CsTenantFederationConfiguration](https://docs.microsoft.com/powershell/module/skype/set-cstenantfederationconfiguration?view=skype-ps&preserve-view=true).
