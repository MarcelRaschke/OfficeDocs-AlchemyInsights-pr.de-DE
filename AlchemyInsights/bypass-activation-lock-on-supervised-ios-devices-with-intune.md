---
title: Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 18c85db8b8fd6179bfb39d0458a5e79a29713ac1
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65735060"
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