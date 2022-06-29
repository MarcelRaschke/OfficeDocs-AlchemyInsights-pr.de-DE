---
title: Application Protection Policy (Anwendungsschutzrichtlinie)
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
- "1073"
ms.date: 07/22/2020
ms.openlocfilehash: 1a255025dac8f46e60cc42752de6b9b74c0d484d
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66261082"
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