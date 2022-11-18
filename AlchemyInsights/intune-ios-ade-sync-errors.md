---
title: Synchronisierungsfehler bei der automatischen Geräteregistrierung von Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 08672beca2903db425c4d1bba3fd91a62d71e0c9
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66375375"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synchronisierungsfehler bei der automatischen Geräteregistrierung von Apple

"Wir haben festgestellt, dass Sie ein oder mehrere ADE/DEP-Token haben, die sich in einem Fehlerzustand befinden. Bis der Fehlerstatus für jedes betroffene Token behoben ist, funktioniert die ADE-Funktionalität nicht wie erwartet."

Dieser Fehler kann auf verschiedene Arten auftreten, z. B.:

1. Geräte werden möglicherweise nicht von ABM/ASM mit Intune
2. Registrierungsprofilzuweisungen können fehlschlagen
3. Geräte können die ADE-Registrierung möglicherweise nicht erfolgreich abschließen.

Überprüfen Sie, ob der Synchronisierungsfehler in der Intune Konsole unter **"Geräte > Geräte registrieren > Apple-Registrierung > Registrierungsprogrammtoken**" gemeldet wurde.

Eine der häufigsten Ursachen für Synchronisierungsfehler ist der Ablauf des aktuellen Tokens. In vielen Fällen wird das Problem durch die Erneuerung des betroffenen Tokens behoben.

Wenn eines oder mehrere Ihrer Token abgelaufen sind, lesen Sie die folgende Dokumentation, um Sie bei bedarfsgemäßer Verlängerung zu unterstützen:

[Erneuern eines Tokens für die automatische Geräteregistrierung](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Darüber hinaus sehen Sie die folgende Dokumentation, um mögliche Korrekturen für andere Fehler anzuzeigen, die Tokensynchronisierungsfehler verursachen:

[ABM/ASM-Synchronisierungsfehler für iOS/iPadOS- und macOS-Automatische Geräteregistrierungstoken](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-Synchronisierungsfehler für iOS/iPadOS- und macOS-Automatische Geräteregistrierungstoken](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
