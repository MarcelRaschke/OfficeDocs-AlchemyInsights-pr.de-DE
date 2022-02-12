---
title: Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräte
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: de6de82cc651580542291e87040d2813db6cb8e3
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62630274"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräte

Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten. Sicherheitsgrundsätze sind vorkonfigurierte Gruppen von Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den relevanten Sicherheitsteams empfohlen werden. Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.

Wenn Sie Sicherheitsgrundwerte für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die auf Windows 10 oder höher ausgeführt werden. Beispielsweise aktiviert MDM Security Baseline (1) BitLocker automatisch für Wechseldatenträger, (2) erfordert das Kennwort zum Entsperren eines Geräts und (3) deaktiviert die Standardauthentifizierung. Wenn eine Standardeinstellung für Ihre Umgebung nicht funktioniert, passen Sie die Baseline so an, dass die benötigten Einstellungen angewendet werden.

Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren. Im Folgenden sind einige Vorteile dieses Vorgangs dargestellt:

- Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen. Da Microsoft Intune mit dem Windows-Sicherheitsteam zusammenarbeitet, das die Grundsätze für Gruppenrichtlinien erstellt, basieren diese Empfehlungen auf soliden Richtlinien und umfangreichen Erfahrungen.
- Wenn Sie neu bei Microsoft Intune sind und nicht wissen, wo Sie anfangen sollen, helfen Ihnen die Sicherheitsgrundsätze dabei, schnell ein sicheres Profil zu erstellen und bereitzustellen.
- Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Intune zu Verwaltungszwecken mit Sicherheitsgrundwerten viel einfacher, da sie in Intune integriert sind und moderne Funktionen für die Verwaltung enthalten.

Weitere Informationen finden Sie [unter Windows Sicherheitsgrundwerte](https://go.microsoft.com/fwlink/?linkid=2141503) und verwaltung [mobiler Geräte](https://go.microsoft.com/fwlink/?linkid=2141701).