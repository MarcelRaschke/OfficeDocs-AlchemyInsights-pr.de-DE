---
title: 0x8004de40 Fehler beim Starten von OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946578"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 Fehler beim Starten von OneDrive

Wenn sie bei der Anmeldung bei OneDrive eine Fehlermeldung **0x8004de40** erhalten, starten Sie den Computer neu, während Sie mit Ihrer Geschäfts-, Schul- oder Unidomäne verbunden sind. Wenn sie nach dem Neustart diesen Fehler erhalten, versuchen Sie es, während Sie mit Ihrer Geschäfts-, Schul- oder Unidomäne verbunden sind:

1. Klicken Sie auf "Start", geben Sie **"cmd"** oder **"Eingabeaufforderung"**  in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabeaufforderungs-App, und wählen Sie  **"Als Administrator ausführen"** aus. Wenn Sie zur Eingabe eines Administratorkennworts oder zur Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **"Zulassen".**  

2. Geben Sie im **Eingabeaufforderungsfenster "dsregcmd /leave"**  ein, und warten Sie, bis der Befehl abgeschlossen ist. Geben Sie dann **dsregcmd /join** ein, und warten Sie, bis der Befehl abgeschlossen ist.
3. Starten Sie Ihren Computer neu.
