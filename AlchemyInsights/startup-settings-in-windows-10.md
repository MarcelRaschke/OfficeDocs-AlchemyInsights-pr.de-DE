---
title: Starteinstellungen in Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909825"
---
# <a name="startup-settings-in-windows-10"></a>Starteinstellungen in Windows 10

**Ändern, welche Apps beim Start automatisch ausgeführt werden**

1. Wechseln Sie zu [Einstellungen > Apps > Start.](ms-settings:startupapps?activationSource=GetHelp)

2. Stellen Sie sicher, dass alle **Apps,** die Sie beim Start ausführen möchten, aktiviert sind.

**Hinzufügen einer App, die beim Start automatisch ausgeführt werden soll**

1. Klicken oder tippen Sie auf **"Start",** und suchen Sie die App, die Sie beim Start ausführen möchten.

2. Klicken Sie mit der rechten Maustaste auf die App, klicken Sie auf **"Mehr",** und klicken Sie dann auf **"Dateispeicherort öffnen".** Dadurch wird der Speicherort geöffnet, an dem die Verknüpfung mit der App gespeichert wird. Wenn keine Option für den Dateispeicherort "Öffnen" vorhanden ist, bedeutet dies, dass die App beim Start nicht ausgeführt werden kann.

3. Wenn der Dateispeicherort geöffnet ist, drücken Sie die **Windows Logo-Taste + R**, geben Sie **shell:startup** ein, und klicken Sie dann auf **OK**. Dadurch wird der Startordner geöffnet.

4. Kopieren Sie die Verknüpfung, und fügen Sie sie aus dem Dateispeicherort in den Startordner in die App ein.

**Erweiterte Startoptionen (einschließlich Tresor Modus, UEFI-Einstellungen und Start von einem anderen Gerät)**

1. Speichern Sie Ihre Arbeit, und schließen Sie alle geöffneten Dokumente, da der PC durch diese Schritte neu gestartet wird.

2. Wechseln Sie zu [Einstellungen > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Klicken Sie unter **"Erweiterter Start"** auf **"Jetzt neu starten".** 

4. Nachdem Ihr PC neu gestartet wurde, wählen Sie einen Optionsbildschirm aus:

    - Klicken Sie zum Starten von einem Gerät wie einem USB-Laufwerk auf **"Gerät verwenden".**

    - Klicken Sie zum Eingeben der UEFI-Einstellungen (manchmal als BIOS-Setup bezeichnet) auf **Problembehandlung > Erweiterten Optionen > UEFI Firmware Einstellungen.** 

    - Um in den Tresor Modus zu wechseln oder erweiterte Starteinstellungen zu ändern, klicken Sie auf **"Problembehandlung > Erweiterte Optionen > Start Einstellungen"** und dann auf **"Neu starten".** Möglicherweise werden Sie aufgefordert, Ihren [BitLocker-Wiederherstellungsschlüssel](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)einzugeben. Klicken Sie nach dem neustarten des PCs auf die Starteinstellung, die Sie verwenden möchten.