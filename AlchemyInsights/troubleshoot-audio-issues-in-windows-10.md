---
title: Behandeln von Audioproblemen in Windows 10
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9001463"
- "3476"
ms.openlocfilehash: c20736a0a8d5929cb2f10057c0014cb365e9aa41
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66345560"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Beheben von Audioproblemen in Windows 10

**Ausführen der Audioproblembehandlung**

1. Öffnen Sie die [Problembehandlungseinstellungen](ms-settings:troubleshoot).

2. Wählen Sie **"Audio** >  wiedergeben"**aus. Führen Sie die Problembehandlung** aus.

**Festlegen des Standardgeräts**

Wenn Sie eine Verbindung mit einem Audiogerät über USB oder HDMI herstellen, müssen Sie dieses Gerät möglicherweise als Standard festlegen:

1. Öffnen **Sie "Start** > **Sound**", und wählen Sie dann **"Sound** " oder **"Systemsounds ändern"** aus der Ergebnisliste aus.

2. Wählen Sie auf der Registerkarte " **Wiedergabe** " ein Gerät aus, wählen Sie **"Standard festlegen"** und dann **"OK**" aus.

**Überprüfen von Kabeln, Lautstärke, Lautsprechern und Kopfhörern**

1. Überprüfen Sie ihre Lautsprecher- und Kopfhörerverbindungen auf lose Kabel, und stellen Sie sicher, dass sie an die richtige Buchse angeschlossen sind.

2. Überprüfen Sie die Energie- und Lautstärkestufen, und versuchen Sie, alle Lautstärkeregler zu erhöhen.

3. Einige Lautsprecher und Apps verfügen über eigene Lautstärkeregler. Möglicherweise müssen Sie sie alle überprüfen, um sicherzustellen, dass sie sich auf den richtigen Ebenen befinden.

4. Versuchen Sie, eine Verbindung über einen anderen USB-Anschluss herzustellen.

**Hinweis**: Denken Sie daran, dass Ihre Lautsprecher möglicherweise nicht funktionieren, wenn Kopfhörer angeschlossen sind.

**Überprüfen Geräte-Manager**

So stellen Sie sicher, dass die Treiber auf dem neuesten Stand sind:

1. Wählen Sie **"Start**" aus, geben **Sie Geräte-Manager** ein, und wählen Sie dann **Geräte-Manager** aus der Ergebnisliste aus.

2. Wählen Sie unter **Sound-, Video- und Gamecontroller** Ihre Soundkarte aus, öffnen Sie sie, wählen Sie die Registerkarte **"Treiber** " und dann **"Treiber aktualisieren"** aus.

**Hinweis**: Wenn Windows keinen neuen Treiber findet, suchen Sie auf der Website des Geräteherstellers nach einem Treiber, und folgen Sie den Anweisungen.

**Installieren Sie den Treiber erneut.**

Wenn Sie nicht über Geräte-Manager aktualisieren oder auf der Website des Herstellers einen neuen Treiber finden können, führen Sie die folgenden Schritte aus:

1. Klicken Sie in Geräte-Manager mit der rechten Maustaste auf den Audiotreiber (oder halten Sie sie gedrückt), und wählen Sie **"Deinstallieren" aus**. Starten Sie Ihr Gerät neu, und Windows versucht, den Treiber neu zu installieren.

2. Wenn das erneute Installieren des Treibers nicht funktioniert, versuchen Sie, den generischen Audiotreiber zu verwenden, der im Lieferumfang von Windows ist. Klicken Sie in Geräte-Manager mit der rechten Maustaste auf Ihre **Audiotreiber-Updatetreibersoftware** \> \> (oder halten Sie sie gedrückt). **Durchsuchen Sie meinen Computer nach Treibersoftware** \> **Lassen Sie mich aus einer Liste der Gerätetreiber auf meinem Computer auswählen**, **High Definition Audio Device** auswählen, **"Weiter**" auswählen und den Anweisungen zum Installieren folgen.
