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
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1f627a92df0cbe162e3f9bab01d290f28907606d
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63235815"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synchronisierungsfehler bei der automatischen Geräteregistrierung von Apple

"Wir haben festgestellt, dass Sie über ein oder mehrere ADE/DEP-Token verfügen, die sich in einem Fehlerstatus befinden. Bis der Fehlerstatus für jedes betroffene Token aufgelöst wurde, funktioniert die ADE-Funktion nicht wie erwartet.".

Dieser Fehler kann auf verschiedene Arten auftreten, z. B.:

1. Geräte dürfen nicht von ABM/ASM mit Intune synchronisiert werden
2. Registrierungsprofilzuweisungen können fehlschlagen
3. Geräte schließen ADE-Registrierung möglicherweise nicht erfolgreich ab

Suchen Sie nach dem Synchronisierungsfehler, der in der Intune-Konsole unter **"Geräte > Geräte registrieren" > Apple-Registrierung >-Registrierungsprogrammtoken** gemeldet wurde.

Eine der häufigsten Ursachen für Synchronisierungsfehler ist der Ablauf des aktuellen Tokens. In vielen Fällen wird das Problem durch die Verlängerung des betroffenen Tokens behoben.

Wenn eines oder mehrere Ihrer Token abgelaufen sind, lesen Sie die folgende Dokumentation, um Sie bei der Verlängerung nach Bedarf zu unterstützen:

[Erneuern eines Tokens für die automatische Geräteregistrierung](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Darüber hinaus finden Sie in der folgenden Dokumentation mögliche Korrekturen für andere Fehler, die zu Fehlern bei der Tokensynchronisierung führen:

[ABM/ASM-Synchronisierungsfehler für iOS/iPadOS und macOS Automatisierte Geräteregistrierungstoken](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM-Synchronisierungsfehler für iOS/iPadOS und macOS Automatisierte Geräteregistrierungstoken](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
