---
title: Application Protection Policy (Anwendungsschutzrichtlinie)
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: c4b2f9635a7c0cfc470ab53e1a041267f7011eae
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63250469"
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