---
title: Chatten Sie mit Benutzern mit Teams persönlichen Konten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9000738"
- "16099"
ms.openlocfilehash: c1e6449b4ebfcf9c0dbd0d11cfb20395cfce3f02
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63300630"
---
# <a name="chat-with-users-with-teams-personal-accounts"></a>Chatten Sie mit Benutzern mit Teams persönlichen Konten

Die Kommunikation mit Benutzern, deren Konten nicht von einer Organisation verwaltet werden (persönliche Konten), ist standardmäßig auf **"Ein** " festgelegt. Administratoren können diese Einstellung für die Organisation aktivieren oder deaktivieren, um zu steuern, ob Benutzer Nachrichten von persönlichen Konten senden oder empfangen können.

1. Wechseln Sie im Teams Admin Center zur Seite "[**UsersExternal**](https://admin.teams.microsoft.com/company-wide-settings/external-communications)  >  Access".
2. Wählen Sie im **Abschnitt Teams Konto, das nicht von einem Organisationsabschnitt verwaltet wird**, den Umschalter aus, um die Einstellung zu deaktivieren oder zu aktivieren.

Weitere Informationen finden Sie unter [Blockieren unerwünschter Kontakte mit externen nicht verwalteten Teams Benutzern](https://docs.microsoft.com/microsoftteams/manage-external-access#block-unsolicited-contact-with-external-unmanaged-teams-users).

Sie können diese Einstellung auch mithilfe von PowerShell verwalten. Einstellungen sind: 

- `CsTenantFederationConfiguration [-AllowTeamsConsumer <Boolean>]` und `[AllowTeamsConsumerInbound]`
- Auf Benutzerebene `CsExternalAccessPolicy [-EnableTeamsConsumerAccess <Boolean>]` und `[-EnableTeamsConsumerInbound <Boolean>]`

Weitere Informationen finden Sie im Referenzhandbuch für [Set-CsTenantFederationConfiguration](https://docs.microsoft.com/powershell/module/skype/set-cstenantfederationconfiguration?view=skype-ps&preserve-view=true).
