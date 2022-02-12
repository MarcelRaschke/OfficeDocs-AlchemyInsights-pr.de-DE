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
ms.openlocfilehash: d59eac9e523c55f32831030f260f1d003de03e68
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62553735"
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

