---
title: Behandeln von Audioproblemen in Windows 10
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 382eb2def9dbaae87a37ec81af75713889acb925
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61963051"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Behandeln von Audioproblemen in Windows 10

**Ausführen der Audioproblembehandlung**

1.  Öffnen Sie die [Problembehandlungseinstellungen.](ms-settings:troubleshoot)

2.  Wählen Sie **"Audio**  >  **wiedergeben" aus, um die Problembehandlung auszuführen.**

**Festlegen des Standardgeräts**

Wenn Sie eine Verbindung mit einem Audiogerät über USB oder HDMI herstellen, müssen Sie dieses Gerät möglicherweise als Standard festlegen:

1. Öffnen **Sie "Sound starten",**  >  und wählen Sie dann **"Sound"** oder **"Systemsound ändern"** aus der Ergebnisliste aus.

2.  Wählen Sie auf der Registerkarte **"Wiedergabe"** ein Gerät aus, wählen Sie **"Standard festlegen"** und dann **"OK"** aus.

**Überprüfen von Kabeln, Lautstärke, Lautsprechern und Kopfhörern**

1. Überprüfen Sie die Lautsprecher- und Kopfhörerverbindungen auf lose Kabel, und stellen Sie sicher, dass sie mit der richtigen Buchse verbunden sind.

2. Überprüfen Sie die Leistungs- und Lautstärkestufen, und versuchen Sie, alle Lautstärkesteuerelemente nach oben zu schalten.

3. Einige Lautsprecher und Apps verfügen über eigene Lautstärkesteuerungen. Möglicherweise müssen Sie alle überprüfen, um sicherzustellen, dass sie auf den richtigen Ebenen sind.

4. Versuchen Sie, eine Verbindung über einen anderen USB-Anschluss herzustellen.

**Hinweis:** Denken Sie daran, dass Ihre Lautsprecher möglicherweise nicht funktionieren, wenn Kopfhörer angeschlossen sind.

**Überprüfen des Geräte-Managers**

So stellen Sie sicher, dass die Treiber auf dem neuesten Stand sind:

1. Wählen Sie **"Start",** geben Sie **"Geräte-Manager"** ein, und wählen Sie dann **"Geräte-Manager"** aus der Liste der Ergebnisse aus.

2. Wählen Sie unter **Sound-, Video- und Gamecontroller** Ihre Soundkarte aus, öffnen Sie sie, wählen Sie die Registerkarte **"Treiber"** und dann **"Treiber aktualisieren" aus.**

**Hinweis:** Wenn Windows keinen neuen Treiber findet, suchen Sie auf der Website des Geräteherstellers nach einem Treiber, und folgen Sie den Anweisungen.

**Erneutes Installieren des Treibers**

Wenn Sie nicht über den Geräte-Manager aktualisieren oder einen neuen Treiber auf der Website des Herstellers finden können, führen Sie die folgenden Schritte aus:

1. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf den Audiotreiber (oder halten Sie den Audiotreiber gedrückt), und wählen Sie **"Deinstallieren" aus.** Starten Sie Ihr Gerät neu, und Windows versucht, den Treiber neu zu installieren.

2. Wenn die Neuinstallation des Treibers nicht funktioniert, versuchen Sie, den generischen Audiotreiber zu verwenden, der im Lieferumfang Windows enthalten ist. Klicken Sie im Geräte-Manager mit der rechten Maustaste auf Ihren Audiotreiber > **Updatetreibersoftware**  >  **Suchen Sie meinen Computer nach Treibersoftware.**  >  **Wählen Sie aus einer Liste der Gerätetreiber auf meinem Computer** aus, wählen Sie **"High Definition Audio Device"** aus, wählen Sie **"Weiter"** aus, und folgen Sie den Anweisungen zur Installation.
