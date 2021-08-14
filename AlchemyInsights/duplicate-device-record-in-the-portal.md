---
title: Doppelter Gerätedatensatz im Portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004153"
---
# <a name="duplicate-device-record-in-the-portal"></a>Doppelter Gerätedatensatz im Portal

Sie sehen möglicherweise zwei Datensätze für ein Gerät im Portal, wenn das Gerät den Co-Verwaltungsstatus nicht korrekt an die Configuration-Manager-Site meldet. Um den Co-Verwaltungsstatus eines Geräts zu überprüfen, überprüfen Sie die Spalte **Co-verwaltet** auf das Gerät in der Configuration Manager-Konsole. Wenn die Spalte nicht sichtbar ist, können Sie sie hinzufügen, indem Sie mit der rechten Maustaste auf eine der Spaltenüberschriften klicken und sie aus der Liste auswählen.

Der Wert für „Co-verwaltet“ muss **Ja** lauten. Wenn er **Nein** lautet, öffnen Sie das Configuration Manager-Client-Applet auf dem Client-Gerät, und aktivieren Sie auf der Registerkarte „Allgemein“ die Eigenschaft **Co-Verwaltung**.

- Wenn der Wert **Aktiviert** lautet, bedeutet dies, dass es Probleme mit der Kommunikation des Clients mit dem Verwaltungspunkt gibt. Bitte lesen Sie auf dem Gerät die Datei **CcmMessaging.log** durch, um mögliche Verbindungsprobleme zu untersuchen.

- Wenn der Wert **Deaktiviert** lautet und das Gerät bei Intune angemeldet ist, stellen Sie bitte sicher, dass das Gerät die Co-Verwaltungsrichtlinie erhalten hat, indem Sie die Datei **CoManagementHandler.log** auf dem Gerät überprüfen.
