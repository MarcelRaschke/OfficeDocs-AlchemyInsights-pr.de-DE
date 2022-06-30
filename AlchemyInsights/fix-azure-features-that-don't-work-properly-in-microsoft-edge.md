---
title: Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 1301794312fd1b003c9ff46c7ac25157cde6397d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66390459"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Vorgehensweise, wenn Azure-Features in Microsoft Edge nicht ordnungsgemäß funktionieren

Microsoft Edge hat [bekannte Probleme](https://go.microsoft.com/fwlink/?linkid=2140608) im Zusammenhang mit Sicherheitszonen und kann sich darauf auswirken, wie sich Azure-Benutzer bei Windows Admin Center anmelden. Wenn Sie Probleme mit der Verwendung von Azure-Features mit Microsoft Edge haben, führen Sie die folgenden Schritte aus:

1. Suchen Sie im **Startmenü** nach **Internetoptionen** , und wählen Sie sie aus.
2. Wechseln Sie im Dialogfeld " **Interneteigenschaften** " zur Registerkarte " **Sicherheit** ".
3. Wählen Sie die Zone **"Vertrauenswürdige Sites** " und dann die Schaltfläche " **Websites** " aus.
4. Fügen Sie im Dialogfeld " **Vertrauenswürdige Websites** " ihre Gateway-URL hinzu [https://login.microsoftonline.com](https://login.microsoftonline.com) , und [https://login.live.com](https://login.live.com)wählen Sie dann " **Schließen**" aus.
5. Wechseln Sie im Dialogfeld " **Interneteigenschaften** " zur Registerkarte " **Datenschutz** ".
6. Wählen Sie im Abschnitt **"Popupblocker** " **die Option "Einstellungen"** aus. Fügen Sie im daraufhin geöffneten Dialogfeld ihre Gateway-URL hinzu [https://login.microsoftonline.com](https://login.microsoftonline.com) , und [https://login.live.com](https://login.live.com)wählen Sie dann **"Schließen**" aus.
