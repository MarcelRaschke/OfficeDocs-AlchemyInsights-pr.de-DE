---
title: Verwenden der Fingerabdruckentsperrungsoption in Windows 10
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: b8750f5d25743d739545e6f4151201aeb129f932
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66523362"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Verwenden der Fingerabdruckentsperrungsoption in Windows 10

**Aktivieren Windows Hello Fingerabdrucks**

Um Windows 10 mit ihrem Fingerabdruck zu entsperren, müssen Sie Windows Hello Fingerabdruck einrichten, indem Sie mindestens einen Finger hinzufügen (damit Windows erkennen kann). 

1. Wechseln **Sie zu Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Die verfügbaren Anmeldeoptionen werden aufgelistet. Zum Beispiel:

    ![Anmeldeoptionen.](media/sign-in-options.png)

2. Klicken oder tippen Sie **auf Windows Hello Fingerabdruck**, und klicken Sie dann auf **"Einrichten**". Klicken Sie im Fenster Windows Hello Setup auf "**Erste Schritte**". Der Fingerabdrucksensor wird aktiviert, und Sie werden aufgefordert, ihren Finger auf dem Sensor zu platzieren:

   ![Fingerabdrucksensor.](media/fingerprint-sensor.png)

3. Befolgen Sie die Anweisungen, in denen Sie aufgefordert werden, Ihren Finger wiederholt zu scannen. Wenn dies abgeschlossen ist, haben Sie die Möglichkeit, weitere Finger hinzuzufügen, die Sie möglicherweise für die Anmeldung verwenden möchten. Wenn Sie sich das nächste Mal bei Windows 10 anmelden, haben Sie die Möglichkeit, dazu Ihren Fingerabdruck zu verwenden.

**Windows Hello Fingerabdruck als Anmeldeoption nicht verfügbar**

Wenn Windows Hello Fingerabdruck in den **Anmeldeoptionen** nicht als Option angezeigt wird, bedeutet dies, dass Windows keinen Fingerabdruckleser/Scanner erkennt, der an Ihren PC angeschlossen ist, oder dass eine Systemrichtlinie die Verwendung verhindert (z. B. wenn Ihr PC von Ihrem Arbeitsplatz verwaltet wird). So behandeln Sie die Problembehandlung: 

1. Wählen Sie die Schaltfläche "**Start**" in der Taskleiste aus, und suchen Sie nach **Geräte-Manager**.

2. Klicken oder tippen Sie, um **Geräte-Manager** zu öffnen.

3. Erweitern Sie in Geräte-Manager biometrische Geräte, indem Sie auf das Chevron klicken.

   ![Biometrische Geräte.](media/biometric-devices.png)

4. Ihr Fingerabdruckscanner sollte als biometrisches Gerät aufgeführt sein, z. B. der Synaptics WBDI-Scanner:

   ![Biometrische Geräte.](media/biometric-devices-expanded.png)

5. Wenn Ihr Fingerabdruckscanner nicht angezeigt wird und der Scanner in Ihren PC integriert ist, wechseln Sie zur Website des PC-Herstellers. Suchen Sie im Abschnitt "Technischer Support" für Ihr PC-Modell nach einem Windows 10 Treiber für einen Scanner, den Sie installieren können.

6. Wenn der Scanner vom PC getrennt ist (über USB angeschlossen), wechseln Sie zur Website des Scannerherstellers, um Windows 10 Gerätetreibersoftware für das Scannermodell zu suchen und zu installieren.
