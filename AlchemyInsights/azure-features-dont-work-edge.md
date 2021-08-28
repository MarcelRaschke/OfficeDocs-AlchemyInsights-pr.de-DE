---
title: Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950323"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren

Microsoft Edge weist bekannte Probleme im Zusammenhang mit Sicherheitszonen auf, die sich auf die Anmeldung von Azure-Benutzern beim Windows Admin Center auswirken können. Weitere Informationen finden Sie unter [Bekannte Probleme in Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Wenn Sie Probleme bei der Verwendung von Azure-Features mit Microsoft Edge haben, versuchen Sie Folgendes:

1. Geben Sie im Startmenü in der **Suchleiste****Internetoptionen** ein, und wählen Sie sie aus.
1. Wählen Sie in **Interneteigenschaften** die Registerkarte **Sicherheit** aus.
1. Wählen Sie **Vertrauenswürdige Sites** und dann **Sites** aus.
1. Fügen Sie Ihre Gateway-URL sowie <https://login.microsoftonline.com> und <https://login.live.com>hinzu, und wählen Sie **Schließen** aus.
1. Wählen Sie in **Interneteigenschaften** die Registerkarte **Datenschutz** aus.
1. Wählen Sie im Abschnitt Popupblocker **Einstellungen** aus. Fügen Sie Ihre Gateway-URL sowie <https://login.microsoftonline.com> und <https://login.live.com>hinzu, und wählen Sie dann **Schließen** aus.