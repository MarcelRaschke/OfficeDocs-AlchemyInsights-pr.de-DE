---
title: Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: af324506f77b12064b9bfff487bbe5cb89fa55b2
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63175423"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren

Microsoft Edge weist bekannte Probleme im Zusammenhang mit Sicherheitszonen auf, die sich auf die Anmeldung von Azure-Benutzern beim Windows Admin Center auswirken können. Weitere Informationen finden Sie unter [Bekannte Probleme in Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Wenn Sie Probleme bei der Verwendung von Azure-Features mit Microsoft Edge haben, versuchen Sie Folgendes:

1. Geben Sie im Startmenü in der **Suchleiste****Internetoptionen** ein, und wählen Sie sie aus.
1. Wählen Sie in **Interneteigenschaften** die Registerkarte **Sicherheit** aus.
1. Wählen Sie **Vertrauenswürdige Sites** und dann **Sites** aus.
1. Fügen Sie Ihre Gateway-URL sowie <https://login.microsoftonline.com> und <https://login.live.com>hinzu, und wählen Sie **Schließen** aus.
1. Wählen Sie in **Interneteigenschaften** die Registerkarte **Datenschutz** aus.
1. Wählen Sie im Abschnitt Popupblocker **Einstellungen** aus. Fügen Sie Ihre Gateway-URL sowie <https://login.microsoftonline.com> und <https://login.live.com>hinzu, und wählen Sie dann **Schließen** aus.