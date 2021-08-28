---
title: Application Protection Policy (Anwendungsschutzrichtlinie)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969970"
---
# <a name="application-protection-policy"></a>Application Protection Policy (Anwendungsschutzrichtlinie)

Wenn Sie mit Application Protection Policy (APP) noch nicht vertraut sind, lesen Sie die [App Protection Policy-Übersicht](https://docs.microsoft.com/intune/apps/app-protection-policy).

Weitere Informationen für die ersten Schritte mit APP finden Sie unter [Erstellen und Zuweisen von App-Schutzrichtlinien](https://docs.microsoft.com/intune/app-protection-policies).

Application Protection Policy – Anforderungen:

- Der Benutzer verfügt über eine Intune- oder EMS-Lizenz.
- Der Benutzer gehört zu einer Gruppe, die durch Anwendungsschutzrichtlinien geschützt ist.
- Nur ein Unternehmensbenutzer ist an geschützten Apps auf einem Gerät angemeldet.
- Für die Anwendung wurde das [Intune-SDK](https://docs.microsoft.com/intune/app-sdk-get-started) implementiert. Eine Liste der Apps, die das SDK unterstützen, finden Sie unter [Geschützte Microsoft Intune-Apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Richtlinien gelten, nachdem sich ein Benutzer, der die vorstehenden Voraussetzungen erfüllt, an einer Intune-SDK-App angemeldet hat. Die einfachste Möglichkeit, um festzustellen, ob eine Richtlinie angewendet wird, besteht darin, dass der Benutzer eine PIN in der Richtlinie festlegen muss. 

Weitere Informationen finden Sie unter:

[App/MAM – häufig gestellte Fragen zur Problembehandlung](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[So überprüfen Sie Ihr Application Protection Policy-Setup](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Grundlegendes zur Bereitstellungszeit für Application Protection Policy](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Überwachen von App-Schutzrichtlinien](https://docs.microsoft.com/intune/app-protection-policies-monitor)