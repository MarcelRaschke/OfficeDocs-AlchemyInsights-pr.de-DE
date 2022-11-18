---
title: Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "6700008"
- "1277"
ms.date: 07/23/2020
ms.openlocfilehash: 965cf27b2c3bb2d91649881469448e4ccedaeaec
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66274420"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune

Die Möglichkeit, die Aktivierungssperre auf iOS-Geräten zu umgehen, erleichtert die Wiederherstellung in dem Szenario, in dem ein Benutzer die Aktivierungssperre auf einem Unternehmensgerät aktiviert und das Unternehmen verlässt.

Zu den Voraussetzungen für die Umgehung einer Aktivierungssperre gehören:

- Das Gerät wird "beaufsichtigt".
- Die Aktivierungssperre wird mithilfe der iOS-Geräteeinschränkungsrichtlinie in Intune erfolgreich aktiviert.

Außerdem sollten Sie beim Umgehen einer Aktivierungssperre:

- das zurückzusetzende Gerät physisch besitzen.
- vor dem Auslösen des Zurücksetzens den Code kopieren.

**Hinweis:** Beim Zurücksetzungscode wird nicht nach Groß-/Kleinschreibung unterschieden, sodass die Zeichen "-"-Zeichen nicht erforderlich sind.

Weitere Informationen finden Sie unter [Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Häufig gestellte Fragen**

F: **Ich habe eine Remoteaktion ausgegeben, um Unternehmensdaten von einem Gerät zu entfernen, und jetzt bleibt es im Status "Ausstehend" hängen.**

A: Damit eine Remoteaktion erfolgreich abgeschlossen werden kann, muss das Zielgerät online und fehlerfrei sein. In den folgenden Situationen bleibt die Remoteaktion 30 Tage lang im Zustand „Ausstehend“ oder bis das Gerät den Befehl bestätigt, falls Folgendes für das Gerät zutrifft:

- Das Gerät hat keine Verbindung.
- Das Gerät verliert seinen Verwaltungsstatus bei Intune.

Wenn Sie der Meinung sind, dass ein Gerät nicht mehr eingecheckt wird und es keine Unternehmensdaten entfernt, wählen Sie "Löschen" aus. Durch das Löschen wird der Gerätedatensatz entfernt, sodass er nicht mehr in der Liste der Geräte in Intune angezeigt wird. Damit das Gerät wieder aktiv wird, muss der Benutzer das Gerät erneut registrieren.

F: **Warum sind bestimmte Remoteaktionen für mich nicht verfügbar?**

A: Nicht alle Plattformen unterstützen alle Remoteaktionen für Geräte. Die folgenden Remoteaktionen sind plattformspezifisch.

- Aktivierungssperre umgehen (nur iOS)
- Sauberer Start (nur Windows)
- Modus für verlorene Geräte (nur iOS)
- Gerät suchen (nur iOS)
- Neustart (nur Windows)

Weitere Details zu den einzelnen Aktionen finden Sie unter [Verfügbare Geräteaktionen](https://docs.microsoft.com/intune/device-management#available-device-actions).