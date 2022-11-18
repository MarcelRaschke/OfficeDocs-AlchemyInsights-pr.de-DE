---
title: Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9004135"
- "7211"
ms.date: 12/03/2020
ms.openlocfilehash: 0297062a4f2634f8c708ec31936ddbf05fdf9f12
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66520185"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten

Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten. Sicherheitsgrundsätze sind vorkonfigurierte Gruppen von Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den relevanten Sicherheitsteams empfohlen werden. Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.

Wenn Sie Sicherheitsbaselines für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die auf Windows 10 oder höher ausgeführt werden. Beispielsweise aktiviert mdm Security Baseline automatisch (1) BitLocker für Wechseldatenträger, (2) erfordert das Kennwort zum Entsperren eines Geräts und (3) deaktiviert die Standardauthentifizierung. Wenn eine Standardeinstellung für Ihre Umgebung nicht funktioniert, passen Sie die Baseline so an, dass die benötigten Einstellungen angewendet werden.

Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren. Im Folgenden sind einige Vorteile aufgeführt:

- Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen. Da Microsoft Intune mit dem Windows-Sicherheitsteam zusammenarbeitet, das die Grundsätze für Gruppenrichtlinien erstellt, basieren diese Empfehlungen auf soliden Richtlinien und umfangreichen Erfahrungen.
- Wenn Sie neu bei Microsoft Intune sind und nicht wissen, wo Sie anfangen sollen, helfen Ihnen die Sicherheitsgrundsätze dabei, schnell ein sicheres Profil zu erstellen und bereitzustellen.
- Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Intune zu Verwaltungszwecken mit Sicherheitsbaselines viel einfacher, da sie in Intune integriert sind und modernste Verwaltungsfunktionen enthalten.

Weitere Informationen finden Sie unter [Windows-Sicherheitsgrundwerte](https://go.microsoft.com/fwlink/?linkid=2141503) und [Mobile Geräteverwaltung](https://go.microsoft.com/fwlink/?linkid=2141701).