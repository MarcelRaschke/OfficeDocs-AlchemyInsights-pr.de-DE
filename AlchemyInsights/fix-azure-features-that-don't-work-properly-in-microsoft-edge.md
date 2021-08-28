---
title: Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117087"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren

Microsoft Edge hat [bekannte Probleme](https://go.microsoft.com/fwlink/?linkid=2140608) im Zusammenhang mit Sicherheitszonen und kann sich darauf auswirken, wie sich Azure-Benutzer bei Windows Admin Center anmelden. Wenn Sie Probleme bei der Verwendung von Azure-Features mit Microsoft Edge haben, führen Sie die folgenden Schritte aus:

1. Suchen Sie im **Startmenü** nach **Internetoptionen,** und wählen Sie sie aus.
2. Wechseln Sie im Dialogfeld **"Interneteigenschaften"** zur Registerkarte **"Sicherheit".**
3. Wählen Sie die Zone **"Vertrauenswürdige Sites"** und dann die Schaltfläche **"Websites"** aus.
4. Fügen Sie im Dialogfeld **"Vertrauenswürdige Websites"** auch die Gateway-URL [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) hinzu, und wählen Sie dann **"Schließen"** aus.
5. Wechseln Sie im Dialogfeld **"Interneteigenschaften"** zur Registerkarte **"Datenschutz".**
6. Wählen Sie im Abschnitt **"Popupblocker"** **Einstellungen** aus. Fügen Sie im daraufhin geöffneten Dialogfeld ihre Gateway-URL [https://login.microsoftonline.com](https://login.microsoftonline.com) hinzu, und [https://login.live.com](https://login.live.com) wählen Sie dann **"Schließen"** aus.
