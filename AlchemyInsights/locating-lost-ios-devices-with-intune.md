---
title: Auffinden verlorener iOS-Geräte mit Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: dabeecaa253cca78dff7b103ee41be4339223243
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62732248"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Auffinden verlorener iOS-Geräte mit Intune

Wenn Sie den Modus für verlorene Geräte auf einem iOS-Gerät aktivieren, kann einem Administrator auf dem Sperrbildschirm eine Nachricht und eine Kontakttelefonnummer angezeigt werden.

Nachdem der Modus für verlorene Geräte aktiviert wurde, kann der Administrator die Aktion „Gerät suchen“ verwenden, um den physischen Standort des Geräts zu identifizieren.

Die Aktion „Gerät suchen“ in Intune funktioniert mit iOS-Geräten, um den Standort eines bestimmten Geräts auf einer Karte anzuzeigen.

Damit diese Aktion verwendet werden kann, muss sich das iOS-Gerät in einem der folgenden Modi befinden:

- Überwachter Modus
- Modus für verlorene Geräte

Weitere Informationen hierzu finden Sie unter [Aktivieren des Modus für verlorene Geräte auf iOS-/iPad-Geräten mit Intune](https://docs.microsoft.com/intune/device-lost-mode) und [Auffinden verlorener oder gestohlener iOS-/iPad-Geräte mit Intune](https://docs.microsoft.com/intune/device-locate).

**Häufig gestellte Fragen**

F: Ich habe eine Remoteaktion zum Entfernen von Unternehmensdaten von einem Gerät gesendet, und jetzt ist das Gerät im Zustand „Ausstehend“ hängen geblieben.

A: Damit eine Remoteaktion erfolgreich abgeschlossen werden kann, muss das Zielgerät online und fehlerfrei sein. In den folgenden Situationen bleibt die Remoteaktion 30 Tage lang im Zustand „Ausstehend“ oder bis das Gerät den Befehl bestätigt:

- Wenn das Gerät keine Verbindung hat.
- Wenn das Gerät seinen Verwaltungsstatus bei Intune verloren hat.

Wenn Sie der Meinung sind, dass das Gerät keinen Check-In mehr vornimmt und dass es nicht mehr in der Lage ist, Unternehmensdaten zu entfernen, wählen Sie „Löschen“ aus. Durch das Löschen wird der Gerätedatensatz entfernt, sodass er nicht mehr in der Liste der Geräte in Intune angezeigt wird. Wenn das Gerät wieder aktiv wird, muss sein Benutzer es erneut registrieren.

F: Warum sind bestimmte Remoteaktionen für mich nicht verfügbar?

A: Nicht alle Plattformen unterstützen alle Remoteaktionen für Geräte. Die folgenden Remoteaktionen sind plattformspezifisch, sodass Sie nur für die aufgeführten Plattformen verfügbar sind.

- Aktivierungssperre umgehen (nur iOS)
- Sauberer Start (nur Windows)
- Modus für verlorene Geräte (nur iOS)
- Gerät suchen (nur iOS)
- Neustart (nur Windows)

Weitere Details zu den einzelnen Aktionen finden Sie unter [Verfügbare Geräteaktionen](https://docs.microsoft.com/intune/device-management#available-device-actions).