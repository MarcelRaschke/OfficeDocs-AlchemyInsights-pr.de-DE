---
title: Überwachen des bedingten Zugriffs
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9003769"
- "6702"
ms.date: 04/21/2020
ms.openlocfilehash: aa951528d3ae83058fe2b40d0323109c7e0b4b0e
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66337455"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Überwachen des bedingten Zugriffs für Exchange

Benutzer, die für bedingten Zugriff bestimmt sind, erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Um die Lösung zu beheben, empfehlen wir eine oder mehrere der folgenden Lösungen:

- Wenn davon ausgegangen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-App zu wechseln und zu überprüfen, ob es in der Unternehmensportal angezeigt wird. Andernfalls sollte der Benutzer das Gerät registrieren.
- Wechseln Sie in der Azure-Portal zu Intune > Gerätekompatibilität. Klicken Sie unter "Überwachen" auf "Gerätekompatibilität". Zeigen Sie ihren Bericht zur Gerätekompatibilität an, um zu überprüfen, ob das Gerät des Benutzers als konform gekennzeichnet ist.
- Wechseln Sie in der Azure-Portal zu Intune > Gerätekompatibilität. Klicken Sie unter "Verwalten" auf "Richtlinien". Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann Intune den Konformitätsstatus des Geräts nicht bestätigen.
- Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.

1. Wechseln Sie in der Azure-Portal zu **Intune** >  Richtlinien für den **zugriffsbereiten Zugriff** > .
2. Wählen Sie eine Richtlinie aus der Liste aus.
3. Klicken Sie auf "Benutzer und Gruppen".
4. Wenn Sie eine bestimmte Richtlinie an eine andere Person adressieren möchten, fügen Sie sie der Liste "Einschließen" hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie sie der Ausschlussliste hinzu.

Nützliche Links:

[Übersicht über die Gerätecompliance](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung bei der Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problembehandlungsrichtlinie](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Überwachen Intune Gerätekompatibilität](https://docs.microsoft.com/intune/compliance-policy-monitor)

Hinweis: Diese Schritte sind nur hilfreich bei der Problembehandlung des bedingten Zugriffs der Azure Active Directory-Funktion. Es ist auch möglich, ein Gerät, das den E-Mail-Zugriff blockiert, mit einer Exchange-Richtlinie zu isolieren. Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [hier](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).
