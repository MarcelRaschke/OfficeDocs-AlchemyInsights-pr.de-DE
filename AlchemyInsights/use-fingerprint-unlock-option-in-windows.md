---
title: Verwenden der Fingerabdruck-Entsperrungsoption in Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 75af465b8ab5c6e4276d816acf78e22dedf1b388
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63177439"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Verwenden der Fingerabdruck-Entsperrungsoption in Windows 10

**Aktivieren Windows Hello Fingerabdrucks**

Um Windows 10 mit ihrem Fingerabdruck zu entsperren, müssen Sie Windows Hello Fingerabdruck einrichten, indem Sie mindestens einen Finger hinzufügen (damit Windows lernen, sie zu erkennen). 

1. Wechseln Sie zu **Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Verfügbare Anmeldeoptionen werden aufgelistet. Beispiel:

    ![Anmeldeoptionen.](media/sign-in-options.png)

2. Klicken oder tippen Sie **auf Windows Hello Fingerabdruck**, und klicken Sie dann auf **"Einrichten**". Klicken Sie im Windows Hello Setupfenster auf **"Erste Schritte"**. Der Fingerabdrucksensor wird aktiviert, und Sie werden aufgefordert, Ihren Finger auf den Sensor zu platzieren:

   ![Fingerabdrucksensor.](media/fingerprint-sensor.png)

3. Folgen Sie den Anweisungen, in denen Sie aufgefordert werden, wiederholt mit dem Finger zu scannen. Nach Abschluss dieses Vorgangs haben Sie die Möglichkeit, weitere Finger hinzuzufügen, die Sie für die Anmeldung verwenden möchten. Wenn Sie sich das nächste Mal bei Windows 10 anmelden, haben Sie die Möglichkeit, dazu Ihren Fingerabdruck zu verwenden.

**Windows Hello Fingerabdruck nicht als Anmeldeoption verfügbar**

Wenn Windows Hello Fingerabdruck nicht als Option in **den Anmeldeoptionen** angezeigt wird, bedeutet dies, dass Windows keinen Fingerabdruckleser/Scanner erkennt, der an Ihren PC angefügt ist, oder dass eine Systemrichtlinie die Verwendung verhindert (z. B. wenn Ihr PC von Ihrem Arbeitsplatz verwaltet wird). So beheben Sie Probleme: 

1. Wählen Sie die **Startschaltfläche** in der Taskleiste aus, und suchen Sie nach **dem Geräte-Manager**.

2. Klicken oder tippen Sie, um den **Geräte-Manager** zu öffnen.

3. Erweitern Sie im Geräte-Manager biometrische Geräte, indem Sie auf das zugehörige Chevron klicken.

   ![Biometrische Geräte.](media/biometric-devices.png)

4. Ihr Fingerabdruckscanner sollte als biometrisches Gerät, z. B. der Synaptics WBDI-Scanner, aufgeführt werden:

   ![Biometrische Geräte.](media/biometric-devices-expanded.png)

5. Wenn Ihr Fingerabdruckscanner nicht angezeigt wird und der Scanner in Ihren PC integriert ist, wechseln Sie zur Website des PC-Herstellers. Suchen Sie im Abschnitt "Technischer Support" für Ihr PC-Modell nach einem Windows 10 Treiber für einen Scanner, den Sie installieren können.

6. Wenn der Scanner vom PC getrennt ist (über USB angeschlossen), wechseln Sie zur Website des Scannerherstellers, um Windows 10 Gerätetreibersoftware für das Scannermodell zu suchen und zu installieren.
