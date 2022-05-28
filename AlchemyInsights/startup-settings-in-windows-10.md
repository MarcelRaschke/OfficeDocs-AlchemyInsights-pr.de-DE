---
title: Starteinstellungen in Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 98bc47833ed6a4979e46afd222ce9e44c8774867
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65732972"
---
# <a name="startup-settings-in-windows-10"></a>Starteinstellungen in Windows 10

**Ändern, welche Apps beim Start automatisch ausgeführt werden**

1. Wechseln Sie zu [Einstellungen > Apps > Start](ms-settings:startupapps?activationSource=GetHelp).

2. Stellen Sie sicher, dass alle Apps, die Sie beim Start ausführen möchten **, aktiviert** sind.

**Hinzufügen einer App, die beim Start automatisch ausgeführt werden soll**

1. Klicken oder tippen Sie auf **"Start** ", und suchen Sie die App, die Sie beim Start ausführen möchten.

2. Klicken Sie mit der rechten Maustaste auf die App, klicken Sie auf **"Mehr**", und klicken Sie dann auf **"Dateispeicherort öffnen"**. Dadurch wird der Speicherort geöffnet, an dem die Verknüpfung mit der App gespeichert wird. Wenn keine Option zum Öffnen des Dateispeicherorts vorhanden ist, bedeutet dies, dass die App beim Start nicht ausgeführt werden kann.

3. Drücken Sie bei geöffnetem Dateispeicherort die **Windows Logo-Taste+R**, geben Sie **"shell:startup**" ein, und klicken Sie dann auf **"OK**". Dadurch wird der Ordner "Start" geöffnet.

4. Kopieren Sie die Verknüpfung mit der App, und fügen Sie sie aus dem Dateispeicherort in den Ordner "Start" ein.

**Erweiterte Startoptionen (einschließlich Tresor Modus, UEFI-Einstellungen und Starten von einem anderen Gerät)**

1. Speichern Sie Ihre Arbeit, und schließen Sie alle geöffneten Dokumente, da diese Schritte ihren PC neu starten.

2. Wechseln Sie zu [Einstellungen > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Klicken Sie unter **"Erweiterter Start**" auf **"Jetzt neu starten**". 

4. Nach dem Neustart des PCs auf dem Optionsbildschirm "Auswählen":

    - Um von einem Gerät wie einem USB-Laufwerk zu starten, klicken Sie auf **"Gerät verwenden"**.

    - Um die UEFI-Einstellungen (manchmal auch ALS BIOS-Setup bezeichnet) einzugeben, klicken Sie auf **Problembehandlung > Erweiterte Optionen > UEFI-Firmware-Einstellungen**. 

    - Um in Tresor Modus zu wechseln oder die erweiterten Starteinstellungen zu ändern, klicken Sie auf **"Problembehandlung > Erweiterte Optionen > Einstellungen starten**", und klicken Sie dann auf **"Neu starten**". Möglicherweise werden Sie aufgefordert, Ihren [BitLocker-Wiederherstellungsschlüssel](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) einzugeben. Nachdem Der PC erneut gestartet wurde, klicken Sie auf die Starteinstellung, die Sie verwenden möchten.