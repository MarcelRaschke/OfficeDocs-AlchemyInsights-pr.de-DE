---
title: Dateien bei Bedarf
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9003530"
- "6432"
ms.date: 07/15/2020
ms.openlocfilehash: d7fb5c2e1c6685325d8ed1a12e90856c444e2811
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66377643"
---
# <a name="configure-files-on-demand"></a>OneDrive-Dateien bei Bedarf konfigurieren

OneDrive-Dateien bei Bedarf benötigt [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (Version 1709 oder höher) oder Windows Server 2019 und OneDrive Build 17.3.7064.1005 oder höher.

Bei neuen OneDrive-Konten unter Mac OS Mojave oder neuer ist Dateien bei Bedarf beim Einrichten von OneDrive standardmäßig aktiviert. Bestehende Benutzer müssen Dateien bei Bedarf in den OneDrive-Einstellungen aktivieren.

[Weitere Informationen zu Dateien bei Bedarf für Mac OS](https://support.microsoft.com/office/529f6d53-e572-4922-a585-e7a318c135f0).

Mit OneDrive-Dateien bei Bedarf können Sie auf alle Ihre Dateien in OneDrive zugreifen, ohne alle herunterladen und Speicherplatz auf Ihrem Gerät nutzen zu müssen.

So konfigurieren Sie die Dateien bei Bedarf auf Ihrem PC:

1. Wählen Sie das weiße oder blaue **OneDrive** Cloudsymbol im Benachrichtigungsbereich der Windows-Taskleiste aus. Wählen Sie **Hilfe & Einstellungen** Zahnradsymbol > **Einstellungen**.
2. Aktivieren Sie auf der Registerkarte **Einstellungen** das Kontrollkästchen **Platz sparen und Dateien erst bei Verwendung herunterladen**.  

Sie können Dateien bei Bedarf auch mithilfe der Registrierung konfigurieren.

Wenn Sie diese Einstellung deaktivieren, tritt für Windows 10-Benutzer das gleiche Synchronisierungsverhalten wie für Benutzer früherer Versionen von Windows auf, und Benutzer können „Dateien bei Bedarf“ nicht aktivieren. Wenn Sie diese Einstellung nicht konfigurieren, können Benutzer „Dateien bei Bedarf“ aktivieren oder deaktivieren.

Durch Aktivieren dieser Richtlinie wird der folgende Registrierungsschlüsselwert auf 1 festgelegt. Das Deaktivieren dieser Richtlinie setzt den folgenden Registrierungsschlüsselwert auf 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Wenn die „Dateien bei Bedarf“-Option in „Einstellungen“ nicht angezeigt wird, stellen Sie sicher, dass der Starttyp des Dienstes „Windows Cloud Files Filter Driver“ auf 2 (AUTO_START) festgelegt ist. Das Aktivieren dieses Features setzt den folgenden Registrierungsschlüsselwert auf 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`
