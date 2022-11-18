---
title: 0x8004de40 Fehler beim Starten von OneDrive
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003837"
- "6886"
ms.openlocfilehash: b99be3aa374e36fa432d72e6363a13d8bf6649f7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66269488"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 Fehler beim Starten von OneDrive

Wenn bei der Anmeldung bei OneDrive **eine Fehlermeldung 0x8004de40** angezeigt wird, starten Sie den Computer neu, während Sie mit Ihrer Geschäfts-, Schul- oder Unidomäne verbunden sind. Wenn diese Fehlermeldung nach dem Neustart angezeigt wird, versuchen Sie es, während Sie mit Ihrer Geschäfts-, Schul- oder Unidomäne verbunden sind:

1. Klicken Sie auf "Start", geben Sie " **CMD** " oder **"Eingabeaufforderung**  " in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabeaufforderungs-App, und wählen Sie "  **Als Administrator ausführen" aus**. Wenn Sie zur Eingabe eines Administratorkennworts oder zur Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **"Zulassen"**.  
2. Geben Sie im **Eingabeaufforderungsfenster "dsregcmd /leave" ein** , und warten Sie, bis der Befehl abgeschlossen ist. Geben Sie dann **dsregcmd /join** ein, und warten Sie, bis der Befehl abgeschlossen ist.
3. Starten Sie Ihren Computer neu.
