---
title: Freigeben von Speicherplatz in Windows 10
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 0d449d0955eb74ba3ad411f0e6db71eb7e5e7ff2
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61946842"
---
# <a name="free-up-drive-space-in-windows-10"></a>Freigeben von Speicherplatz in Windows 10

Hier finden Sie zwei Optionen, um Speicherplatz in Windows freizugeben:

- Geben Sie Speicherplatz in Windows 10 frei.
- Geben Sie Speicherplatz für Windows 10-Updates mit einem externen Speichergerät frei.

Wenn Sie nach der Verwendung der Datenträgerbereinigung immer noch wenig Speicherplatz haben, füllt sich Ihr Ordner für temporäre Dateien möglicherweise schnell mit Anwendungsdateien (.appx), die vom Microsoft Store verwendet werden. Um dieses Problem zu beheben, setzen Sie den Store zurück, löschen Sie den Store-Cache und führen Sie dann die Windows Update-Problembehandlung durch. Stellen Sie sicher, dass der Microsoft Store geschlossen ist, bevor Sie mit diesen Schritten fortfahren.

**Schritt 1: Zurücksetzen des Microsoft Store**

**Hinweis**: Dies löscht die App-Daten auf dem Gerät endgültig, einschließlich Ihrer Einstellungen und Anmeldedetails.

1. Wählen Sie **Start** > **Einstellungen** > **Apps** > **Apps & Features** aus.

1. Suchen Sie in der Liste der Apps den Microsoft Store und wählen Sie ihn aus.

1. Wählen Sie **Erweiterte Optionen** aus.

1. Blättern Sie nach unten und wählen Sie **Zurücksetzen** aus und dann **Zurücksetzen bestätigen**.

**Schritt 2: Löschen des Microsoft Store-Cache**

1. Drücken Sie die WINDOWS-TASTE+R, um das Dialogfeld „Ausführen“ zu öffnen.

1. Geben Sie wsreset.exe ein und wählen Sie **OK**.

1. Ein leeres Eingabeaufforderungsfenster wird geöffnet. Nach ungefähr 10 Sekunden schließt sich das Fenster und der Store wird automatisch geöffnet.

**Schritt 3: Zurücksetzen von Windows Update**

1. Wählen Sie **Start** > **Einstellungen** > **Update & Sicherheit** > **Problembehandlung** aus.

1. Blättern Sie nach unten und wählen Sie **Windows Update** aus der Liste aus, und wählen Sie **Problembehandlung ausführen** aus.

1. Starten Sie Ihren Computer neu und prüfen Sie, ob das Problem weiterhin auftritt.

