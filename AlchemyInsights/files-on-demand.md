---
title: Dateien bei Bedarf
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.date: 07/15/2020
ms.openlocfilehash: f6c6409319f617fa5eefa1a36977f3d64d3ae73f
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62576883"
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

Wenn Sie diese Einstellung deaktivieren, weisen Windows 10-Benutzer das gleiche Synchronisierungsverhalten wie Benutzer der früheren Versionen von Windows auf, und sie können "Dateien bei Bedarf" nicht aktivieren. Wenn Sie diese Einstellung nicht konfigurieren, können die Benutzer „Dateien bei Bedarf“ aktivieren oder deaktivieren.

Durch Aktivieren dieser Richtlinie wird der folgende Registrierungsschlüsselwert auf 1 festgelegt. Das Deaktivieren dieser Richtlinie setzt den folgenden Registrierungsschlüsselwert auf 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Wenn die Dateien bei Bedarf-Option in „Einstellungen“ nicht angezeigt wird, stellen Sie sicher, dass der Starttyp des Dienstes „Windows-Clouddateien-Filter-Treiber“ auf 2 (AUTO_START) festgelegt ist. Das Aktivieren dieses Features setzt den folgende Registrierungsschlüsselwert auf 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`
