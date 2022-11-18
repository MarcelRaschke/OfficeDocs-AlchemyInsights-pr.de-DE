---
title: Hinzufügen externer Mitglieder zu freigegebenen Kanälen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9011182"
- "18175"
ms.openlocfilehash: 7120efda4948c19bbbc03b73b268e78bfce8f80c
ms.sourcegitcommit: 257eca543d955d79eb9591b88b9101f07c8dadbf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/08/2022
ms.locfileid: "67629629"
---
# <a name="add-external-members-on-shared-channels"></a>Hinzufügen externer Mitglieder zu freigegebenen Kanälen

Führen Sie die folgenden Schritte aus, um Richtlinien zum Hinzufügen externer Benutzer zu freigegebenen Kanälen zu konfigurieren:

1. Stellen Sie sicher, dass der Benutzer über die entsprechende TeamsChannelPolicy verfügt, um externe Benutzer zu freigegebenen Kanälen einzuladen. Weitere Informationen finden [Sie unter Verwalten von Kanalrichtlinien in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/teams-policies).
1. Stellen Sie sicher, dass die Azure B2B Direct Connect-Richtlinie für Ihre Mandanten und Partnermandanten eingerichtet wurde. Weitere Informationen finden Sie unter [Konfigurieren des mandantenübergreifenden Zugriffs von B2B Direct Connect](https://docs.microsoft.com/azure/active-directory/external-identities/cross-tenant-access-settings-b2b-direct-connect).
1. Stellen Sie sicher, dass der B2B-Gastzugriff in Ihrem Mandanten aktiviert ist. Weitere Informationen finden Sie unter [Konfigurieren des mandantenübergreifenden Zugriffs für die B2B-Zusammenarbeit](https://docs.microsoft.com/azure/active-directory/external-identities/cross-tenant-access-settings-b2b-collaboration). 

**Hinweise**:

- Änderungen an mandantenübergreifenden Zugriffseinstellungen können bis zu sechs Stunden dauern, bis sie wirksam werden. Weitere Informationen finden Sie [unter Limit who can be invited by an organization](https://docs.microsoft.com/microsoft-365/solutions/limit-invitations-from-specific-organization).
- Nur Besitzer freigegebener Kanäle können Mitglieder zu freigegebenen Kanälen hinzufügen und daraus entfernen. Teams-Besitzer können diese Aktionen nicht ausführen, da jeder freigegebene Kanal über eine eigene Mitgliedschaft verfügt.