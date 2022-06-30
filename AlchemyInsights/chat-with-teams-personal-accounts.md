---
title: Chatten mit Benutzern mit persönlichen Teams-Konten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000738"
- "16099"
ms.openlocfilehash: 261eae8e226ef7b27a112886edf2690cb5de1896
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66394851"
---
# <a name="chat-with-users-with-teams-personal-accounts"></a>Chatten mit Benutzern mit persönlichen Teams-Konten

Die Kommunikation mit Benutzern, deren Konten nicht von einer Organisation verwaltet werden (persönliche Konten), ist standardmäßig auf **"Ein** " festgelegt. Administratoren können diese Einstellung für die Organisation aktivieren oder deaktivieren, um zu steuern, ob Benutzer Nachrichten von persönlichen Konten senden oder empfangen können.

1. Wechseln Sie im Teams Admin Center zur  >  Seite "[**Externer Benutzerzugriff**](https://admin.teams.microsoft.com/company-wide-settings/external-communications)".
2. Wählen Sie im Abschnitt " **Teams-Konto, das nicht von einer Organisation verwaltet wird** " den Umschalter aus, um die Einstellung zu deaktivieren oder zu aktivieren.

Weitere Informationen finden Sie unter [Blockieren eines unerwünschten Kontakts mit externen nicht verwalteten Teams-Benutzern](https://docs.microsoft.com/microsoftteams/manage-external-access#block-unsolicited-contact-with-external-unmanaged-teams-users).

Sie können diese Einstellung auch mithilfe von PowerShell verwalten. Einstellungen sind: 

- `CsTenantFederationConfiguration [-AllowTeamsConsumer <Boolean>]` und `[AllowTeamsConsumerInbound]`
- auf Benutzerebene und `CsExternalAccessPolicy [-EnableTeamsConsumerAccess <Boolean>]``[-EnableTeamsConsumerInbound <Boolean>]`

Weitere Informationen finden Sie im Referenzhandbuch für [Set-CsTenantFederationConfiguration](https://docs.microsoft.com/powershell/module/skype/set-cstenantfederationconfiguration?view=skype-ps&preserve-view=true).
