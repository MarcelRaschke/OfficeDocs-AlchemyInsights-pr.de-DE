---
title: Android-Anwendungsschutzrichtlinie (APP)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "6700006"
- "12456"
ms.date: 06/02/2022
ms.openlocfilehash: 4c2d571b9094f9398166faa600449a9f6f8b1b96
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66301926"
---
# <a name="android-application-protection-policy-app"></a>Android-Anwendungsschutzrichtlinie (APP)

Wenn Sie die Application Protection Policy (APP) noch nicht kennen, lesen Sie den [Überblick über die Application Protection Policies](https://docs.microsoft.com/mem/intune/apps/app-protection-policy).

Weitere Informationen für die ersten Schritte mit APP finden Sie unter [Erstellen und Zuweisen von App-Schutzrichtlinien](https://docs.microsoft.com/intune/app-protection-policies).

Die für die APP verfügbaren Einstellungen hängen von der verwendeten Client-Plattform ab. Android-spezifische APP-Einstellungen finden Sie [unter Android-App-Schutzrichtlinieneinstellungen in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/app-protection-policy-settings-android).

Beachten Sie, dass APP diese Anforderungen erfüllt:

- Der Benutzer muss über eine Intune- oder EMS-Lizenz verfügen.
- Der Benutzer gehört zu einer Gruppe, die durch Anwendungsschutzrichtlinien geschützt ist.
- Nur ein Unternehmensbenutzer ist an geschützten Apps auf einem Gerät angemeldet.
- Für die Anwendung wurde das [Intune-SDK](https://docs.microsoft.com/intune/app-sdk-get-started) implementiert. Eine Liste der Apps, die das SDK unterstützen, finden Sie unter [Geschützte Microsoft Intune-Apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Anwendungsschutzrichtlinien werden erst angewendet, nachdem sich ein Benutzer, der die oben genannten Anforderungen erfüllt, bei einer Intune SDK-aktivierten Anwendung auf dem Gerät unterschrieben hat. Die einfachste Möglichkeit, um festzustellen, ob eine Richtlinie angewendet wird, besteht darin, dass der Benutzer eine PIN in der Richtlinie festlegen muss.

Weitere Informationen finden Sie unter:

- [Behandeln von Problemen mit Benutzern von App-Schutzrichtlinien](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-mam)
- [Problembehandlung bei der Bereitstellung von App-Schutzrichtlinien in Intune](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-protection-policy-deployment)
- [So validieren Sie die Einrichtung Ihrer Anwendungsschutzrichtlinie in Microsoft Intune](https://docs.microsoft.com/intune/app-protection-policies-validate)
- [Grundlegendes zur Bereitstellungszeit für Application Protection Policy](https://docs.microsoft.com/intune/app-protection-policy-delivery)
- [Überwachen von App-Schutzrichtlinien](https://docs.microsoft.com/intune/app-protection-policies-monitor)
