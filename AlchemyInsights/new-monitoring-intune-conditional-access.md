---
title: Überwachen des bedingten Intune-Zugriffs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: c2a750f63a169c4b5151328450c111ce22f29a9f
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62551287"
---
# <a name="monitor-intune-conditional-access"></a>Überwachen des bedingten Intune-Zugriffs

Benutzer, die auf bedingten Zugriff abzielen, erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Um die Lösung zu beheben, empfehlen wir eine oder mehrere der folgenden Lösungen:

1. Wenn davon ausgegangen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal App zu wechseln und zu überprüfen, ob es im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall ist, muss der Benutzer das Gerät registrieren.
1. Wechseln Sie im Azure-Portal zur **IntuneDevice-Compliance** > . 
1. Klicken Sie unter **"Überwachen**" auf " **Gerätekompatibilität**", um den Bericht zur Gerätekompatibilität anzuzeigen, um zu überprüfen, ob das Gerät des Benutzers als kompatibel gekennzeichnet ist.
1. Wechseln Sie im Azure-Portal zur **IntuneDevice-Compliance** > . Klicken Sie unter **"Verwalten** " auf **"Richtlinien**". Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann Intune den Kompatibilitätsstatus des Geräts nicht bestätigen.
1. Bearbeiten Sie die Zuweisung des bedingten Zugriffs des Benutzers.
1. Navigieren Sie im Azure-Portal zu **IntuneConditional** >  **accessPolicies** > , wählen Sie eine Richtlinie aus der Liste aus, und klicken Sie auf **"Benutzer und Gruppen**".
1. Wenn Sie eine bestimmte Richtlinie an jemanden adressieren möchten, fügen Sie sie der **Include-Liste hinzu**. Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie sie der **Liste "Ausschließen" hinzu**.

**Nützliche Links:**

- [Übersicht über die Gerätekompatibilität](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problembehandlung durch Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Problembehandlungsrichtlinie](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Überwachen der Intune-Gerätekompatibilität](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Hinweis**: Diese Schritte sind nur bei der Problembehandlung beim bedingten Azure Active Directory-Feature hilfreich. Es ist auch möglich, ein Gerät unter Quarantäne zu stellen, das den E-Mail-Zugriff mit Exchange Richtlinie blockiert. Weitere Informationen Exchange Geräteverwaltung finden Sie [**hier**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
