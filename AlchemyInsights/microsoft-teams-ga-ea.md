---
title: Microsoft Teams – Gastzugriff
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 91fb4d0e132f7d23f02da2b62264a175d56c244c
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65735420"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams – Gastzugriff

Wenn Sie Hilfe bei der Kommunikation mit Benutzern außerhalb Ihrer Organisation in Teams benötigen, müssen Sie entscheiden, ob Sie [den Gastzugriff oder den externen Zugriff (Verbund)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) verwenden oder beides verwenden möchten.

Überprüfen Sie [unbedingt die Unterschiede](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) , um die jeweils verfügbaren Features zu verstehen.  Der externe Zugriff (Verbund) ermöglicht z. B. 1:1-Kommunikation, z. B. Chat und Anwesenheit.  Verbundbenutzer können jedoch nicht an Teams Zusammenarbeit teilnehmen.  Wenn Sie möchten, dass ein externer Benutzer an Teams Kanalunterhaltungen oder "Dateien freigeben" teilnimmt, müssen Sie den Gastzugriff aktivieren.

**Option 1: Gastzugriff aktivieren** Wechseln Sie im Teams Admin Center zu ["Organisationsweites Einstellungen > Gastzugriff](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration)", und aktivieren Sie "Gastzugriff in Teams zulassen".  Für einen Mandanten mit allen anderen Standardeinstellungen sollte dies alles sein, was Sie tun müssen.  Um Ihre Gastzugriffskonfiguration anzupassen, stellen Sie sicher, dass Sie alle Schritte in der [Checkliste für den Gastzugriff](https://docs.microsoft.com/microsoftteams/guest-access-checklist) ausführen. Sobald Sie fertig sind, müssen Sie [bis zu 24 Stunden warten](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) , bis die Einstellungen wirksam werden.

Wenn Sie sicher sind, dass Sie alle Schritte in der Checkliste abgeschlossen haben und es mehr als 24 Stunden war, fahren Sie fort, und versuchen Sie, [einen Gast zu Ihrem Team hinzuzufügen](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Weitere Informationen, einschließlich Anleitungsvideos, finden [Sie unter Gastzugriff in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Option 2: Aktivieren des externen Zugriffs (Partnerverbund)** Wenn Sie auch den externen Zugriff (Partnerverbund) aktivieren möchten, wechseln Sie im Teams Admin Center zum [organisationsweiten Einstellungen > externen Zugriff](https://admin.teams.microsoft.com/company-wide-settings/external-communications), aktivieren Sie "Benutzer können mit Skype for Business und Teams Benutzern kommunizieren", und führen Sie dann alle Schritte unter ["Lassen Sie Ihre Teams  Benutzer chatten und mit Benutzern in einer anderen Organisation kommunizieren](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).
