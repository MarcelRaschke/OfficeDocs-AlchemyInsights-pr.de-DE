---
title: Überwachen Intune bedingten Zugriffs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004636"
- "8386"
ms.date: 02/25/2021
ms.openlocfilehash: d720f8279a90593d279fcdd10aa9c800265dc3b7
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66364548"
---
# <a name="monitor-intune-conditional-access"></a>Überwachen Intune bedingten Zugriffs

Benutzer, die für bedingten Zugriff bestimmt sind, erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Um die Lösung zu beheben, empfehlen wir eine oder mehrere der folgenden Lösungen:

1. Wenn davon ausgegangen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-App zu wechseln und zu überprüfen, ob es in der Unternehmensportal angezeigt wird. Andernfalls muss der Benutzer das Gerät registrieren.
1. Wechseln Sie in der Azure-Portal zu **Intune** >  **Device-Compliance**. 
1. Klicken Sie unter **"Überwachen**" auf " **Gerätekompatibilität**", um zu überprüfen, ob das Gerät des Benutzers als konform gekennzeichnet ist.
1. Wechseln Sie in der Azure-Portal zu **Intune** >  **Device-Compliance**. Klicken Sie unter **"Verwalten** " auf **"Richtlinien"**. Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann Intune den Konformitätsstatus des Geräts nicht bestätigen.
1. Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.
1. Navigieren Sie in der Azure-Portal zu **Intune** >  Richtlinien für **den zugriff** > , wählen Sie eine Richtlinie aus der Liste aus, und klicken Sie auf **"Benutzer und Gruppen**".
1. Wenn Sie eine bestimmte Richtlinie an eine andere Person adressieren möchten, fügen Sie sie der **Liste "Einschließen"** hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie sie der **Ausschlussliste** hinzu.

**Nützliche Links:**

- [Übersicht über die Gerätecompliance](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problembehandlung bei der Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Problembehandlungsrichtlinie](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Überwachen Intune Gerätekompatibilität](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Hinweis**: Diese Schritte sind nur hilfreich bei der Problembehandlung des bedingten Zugriffs der Azure Active Directory-Funktion. Es ist auch möglich, ein Gerät, das den E-Mail-Zugriff blockiert, mit einer Exchange-Richtlinie zu isolieren. Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [**hier**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
