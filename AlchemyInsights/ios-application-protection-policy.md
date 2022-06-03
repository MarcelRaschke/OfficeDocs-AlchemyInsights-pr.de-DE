---
title: iOS Anwendungsschutzrichtlinie (APP)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "12455"
- "6700006"
ms.date: 06/02/2022
ms.openlocfilehash: 113ca60ec224ca2dbff064444182746658d9f0a9
ms.sourcegitcommit: 29aa28c4fa26e71de062cb6319e48cd963fdf1fc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/03/2022
ms.locfileid: "65862183"
---
# <a name="ios-application-protection-policy-app"></a>iOS Anwendungsschutzrichtlinie (APP)

Wenn Sie die Application Protection Policy (APP) noch nicht kennen, lesen Sie den [Überblick über die Application Protection Policies](https://docs.microsoft.com/mem/intune/apps/app-protection-policy).

Weitere Informationen für die ersten Schritte mit APP finden Sie unter [Erstellen und Zuweisen von App-Schutzrichtlinien](https://docs.microsoft.com/intune/app-protection-policies).

Die für die APP verfügbaren Einstellungen hängen von der verwendeten Client-Plattform ab. Informationen zu iOS-spezifischen APP-Einstellungen finden Sie unter [iOS-App-Schutzrichtlinieneinstellungen](https://docs.microsoft.com/mem/intune/apps/app-protection-policy-settings-ios).

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
