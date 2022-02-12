---
title: Automatische Bereinigung veralteter Geräte in Intune
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: ad133653293c7b91e12cde203bbf70b5f83c7325
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62594460"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatische Bereinigung veralteter Geräte in Intune

Intune erlaubt es dem Administrator, ein Zeitintervall zwischen 90 und 270 Tagen zu konfigurieren, nach dem veraltete Geräte aus dem Dienst entfernt werden. Diese Einstellung gilt organisationsweit wird nach ihrer Aktivierung sofort wirksam. Alle Geräte, die über einen Zeitraum, der die Einstellung überschreitet, keinen Check-In beim Intune-Server durchgeführt haben, werden endgültig gelöscht.

**Hinweis**: Nur MDM-Geräteobjekte sind für diese Bereinigungsaktion berechtigt. Reine EAS-Geräteobjekte sind davon ausgeschlossen.

Weitere Informationen, wann ein Gerät für die Löschung berechtigt wird, basierend auf der Einstellung für die Gerätebereinigung und seinem „Zustand“:

Einstellung: **Geräte nach Datum des letzten Check-Ins löschen: Ja (ein Wert (N), Angabe in Tagen)**

- Basierend auf dem in der Einstellung konfigurierten Wert (N) löscht der Intune-Dienst das Gerät innerhalb der angegebenen Tagen, nachdem es zuletzt erfolgreich eingecheckt wurde.

Einstellung: **Geräte nach Datum des letzten Check-Ins löschen: Nein**

- 180 Tage nachdem das Gerätezertifikat abgelaufen ist und nicht verlängert wurde, wird das Gerät gelöscht.

**Hinweis**: In beiden Fällen muss das Gerät erfolgreich bei Intune registriert sein. Die Registrierung erfolgt während des ersten Check-Ins des Geräts beim Intune-Dienst.

Wird ein Gerät erfolgreich bei Intune registriert, aber nicht Intune-registriert, wird das Gerät 270 Tage nach seiner Registrierung gelöscht. (90 Tage, um das Gerät als „Aufgehoben“ zu markieren, und dann weitere 180 Tage, um den Datensatz zu löschen.)

Zurzeit gibt es in der Intune-Konsole keinen Mechanismus zum Festlegen des Ablaufdatums der Gerätezertifizierung für ein bestimmtes Gerät.