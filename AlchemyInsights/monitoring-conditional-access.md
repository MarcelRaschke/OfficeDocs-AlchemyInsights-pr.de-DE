---
title: Überwachen des bedingten Zugriffs
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975100"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Überwachen des bedingten Zugriffs auf Exchange

Benutzer, die auf bedingten Zugriff abzielen, erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Um die Lösung zu beheben, empfehlen wir eine oder mehrere der folgenden Lösungen:

- Wenn davon ausgegangen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal App zu wechseln und zu überprüfen, ob es im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.
- Wechseln Sie im Azure-Portal zu Intune > Gerätekompatibilität. Klicken Sie unter "Überwachen" auf "Gerätekompatibilität". Zeigen Sie Ihren Bericht zur Gerätekompatibilität an, um zu überprüfen, ob das Gerät des Benutzers als kompatibel gekennzeichnet ist.
- Wechseln Sie im Azure-Portal zu Intune > Gerätekompatibilität. Klicken Sie unter "Verwalten" auf "Richtlinien". Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann Intune den Kompatibilitätsstatus des Geräts nicht bestätigen.
- Bearbeiten Sie die Zuweisung des bedingten Zugriffs des Benutzers.

1. Wechseln Sie im Azure-Portal zu  >  **Intune-Richtlinien für bedingten**  >  Zugriff.
2. Wählen Sie eine Richtlinie aus der Liste aus.
3. Klicken Sie auf "Benutzer und Gruppen".
4. Wenn Sie eine bestimmte Richtlinie an jemanden adressieren möchten, fügen Sie sie der Include-Liste hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie sie der Liste "Ausschließen" hinzu.

Hilfreiche Links:

[Übersicht über die Gerätekompatibilität](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung durch Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problembehandlungsrichtlinie](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Überwachen der Intune-Gerätekompatibilität](https://docs.microsoft.com/intune/compliance-policy-monitor)

Hinweis: Diese Schritte sind nur bei der Problembehandlung für die Azure Active Directory Feature bedingter Zugriff hilfreich. Es ist auch möglich, ein Gerät, das den E-Mail-Zugriff blockiert, mit Exchange Richtlinie unter Quarantäne zu stellen. Weitere Informationen zu Exchange Geräteverwaltung finden Sie [hier]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
