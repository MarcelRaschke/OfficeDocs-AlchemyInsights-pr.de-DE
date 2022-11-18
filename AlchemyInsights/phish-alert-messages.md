---
title: 2491 Warnungs-E-Mail-Nachrichten aus der Richtlinie "Phishing aufgrund von Mandanten- oder Benutzerüberschreibung übermittelt"
ms.author: chrisda
author: chrisda
manager: dansimp
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom: 2491
ms.date: 04/21/2020
ms.openlocfilehash: 1e8a0ecd899c66c510387b4a7dcff07ab7bca7c4
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66255896"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Warnungs-E-Mail-Nachrichten aus der Richtlinie "Phishing aufgrund von Mandanten- oder Benutzerüberschreibung übermittelt"

In Organisationen mit Microsoft Defender für Office 365 P1- und P2-Lizenzen ist eine Standardwarnungsrichtlinie namens **"Phishing zugestellt aufgrund von Mandanten- oder Benutzerüberschreibung**" verfügbar. Wenn Sie diese Warnung erhalten haben, gehen Sie folgendermaßen vor:

1. Klicken Sie in der Warnmeldung auf "**Warnung anzeigen**", um zur Seite "**Benachrichtigungen**" im Microsoft 365 Defender Portal zu wechseln.

2. Wählen Sie die Warnung aus, um die Option zum **Anzeigen der Nachrichtenliste** oder **zum Anzeigen von Nachrichten im Explorer anzuzeigen**. Beide Optionen führen Sie zu den Details der Nachricht, die die Nachrichten-ID enthält. Beachten Sie, dass der Link "Bedrohungs-Explorer" automatisch die Nachrichten filtert, die den Warnungskriterien entsprechen. Möglicherweise müssen Sie den Datumsfilter im Bedrohungs-Explorer anpassen.

Die Phishingnachricht wurde aufgrund einer manuell konfigurierten Außerkraftsetzung zugestellt:

- Ein zulässiger Absender oder eine vom Benutzer festgelegte Domäne.
- Ein zulässiger Absender oder eine vom Administrator in einer Antispamrichtlinie festgelegte Domäne.
- Eine zulässige IP-Adresse in einer Verbindungsfilterrichtlinie.
- Eine Nachrichtenflussregel (auch als Transportregel bezeichnet), die so konfiguriert ist, dass Nachrichten zugelassen werden.

Wenn Sie glauben, dass die Nachricht fälschlicherweise als Phishing gekennzeichnet wurde, verwenden Sie [Admin Übermittlung](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission), um die Nachricht an Microsoft zu melden.

Benutzer können das [Add-In "Nachricht melden" oder das Add-In "Phishing melden"](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) in Outlook verwenden, um Nachrichtenbeispiele an Microsoft zu übermitteln.
