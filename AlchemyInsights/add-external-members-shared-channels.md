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
ms.openlocfilehash: 5dd9df25dfdbb39c71263129008cbc9226172874
ms.sourcegitcommit: 88adb5a8ce6c6cdcda5b28796aad30c5d13fb02b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/07/2022
ms.locfileid: "67618740"
---
# <a name="add-external-members-on-shared-channels"></a>Hinzufügen externer Mitglieder zu freigegebenen Kanälen

Führen Sie die folgenden Schritte aus, um Richtlinien zum Hinzufügen externer Benutzer zu freigegebenen Kanälen zu konfigurieren:

1. Stellen Sie sicher, dass der Benutzer über die entsprechende TeamsChannelPolicy verfügt, um externe Benutzer zu freigegebenen Kanälen einzuladen. Weitere Informationen finden [Sie unter Verwalten von Kanalrichtlinien in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/teams-policies).
1. Stellen Sie sicher, dass die Azure B2B Direct Connect-Richtlinie für Ihre Mandanten und Partnermandanten eingerichtet wurde. Weitere Informationen finden Sie unter [Konfigurieren des mandantenübergreifenden Zugriffs von B2B Direct Connect]()
1. Stellen Sie sicher, dass der B2B-Gastzugriff in Ihrem Mandanten aktiviert ist. Weitere Informationen finden Sie unter [Konfigurieren des mandantenübergreifenden Zugriffs für die B2B-Zusammenarbeit]() 

**Hinweise**:

- Änderungen an mandantenübergreifenden Zugriffseinstellungen können bis zu sechs Stunden dauern, bis sie wirksam werden. Weitere Informationen finden Sie [unter Limit who can be invited by an organization](https://docs.microsoft.com/microsoft-365/solutions/limit-invitations-from-specific-organization).
- Nur Besitzer freigegebener Kanäle können Mitglieder zu freigegebenen Kanälen hinzufügen und daraus entfernen. Teams-Besitzer können diese Aktionen nicht ausführen, da jeder freigegebene Kanal über eine eigene Mitgliedschaft verfügt.