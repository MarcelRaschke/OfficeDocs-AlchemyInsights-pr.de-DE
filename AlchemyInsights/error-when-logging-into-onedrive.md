---
title: 0x8004de40 Fehler beim Starten von OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: abae00278c1dc8fc64df061d3788c3a22cadb1e2
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65724360"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 Fehler beim Starten von OneDrive

Wenn beim Anmelden bei OneDrive eine Fehlermeldung **0x8004de40** angezeigt wird, starten Sie den Computer neu, während Sie mit Ihrer Geschäfts-, Schul- oder Unidomäne verbunden sind. Wenn diese Fehlermeldung nach dem Neustart angezeigt wird, versuchen Sie es, während Sie mit Ihrer Geschäfts-, Schul- oder Unidomäne verbunden sind:

1. Klicken Sie auf "Start", geben Sie " **CMD** " oder **"Eingabeaufforderung**  " in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabeaufforderungs-App, und wählen Sie "  **Als Administrator ausführen" aus**. Wenn Sie zur Eingabe eines Administratorkennworts oder zur Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **"Zulassen"**.  
2. Geben Sie im **Eingabeaufforderungsfenster "dsregcmd /leave" ein** , und warten Sie, bis der Befehl abgeschlossen ist. Geben Sie dann **dsregcmd /join** ein, und warten Sie, bis der Befehl abgeschlossen ist.
3. Starten Sie Ihren Computer neu.
