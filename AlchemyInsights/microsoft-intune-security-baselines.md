---
title: Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräte
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 8ce37d1e11f8495a0980d4ad58a6438d83bffef7
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62667319"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräte

Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten. Sicherheitsgrundwerte sind Windows vorkonfigurierte Gruppen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den entsprechenden Sicherheitsteams empfohlen werden. Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.

Wenn Sie Sicherheitsgrundwerte für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die auf Windows 10 oder höher ausgeführt werden. Beispielsweise aktiviert die Microsoft Mobile Device Management (MDM)-Sicherheitsbaseline BitLocker automatisch für Wechseldatenträger, erfordert das Kennwort zum Entsperren eines Geräts und deaktiviert die Standardauthentifizierung. Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, können Sie die Grundsätze anpassen, um die gewünschten Einstellungen anzuwenden.

Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren. Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen. Intune arbeitet mit dem Windows Sicherheitsteam zusammen, das Basispläne für Gruppenrichtlinien erstellt. Daher basieren diese Empfehlungen auf soliden Anleitungen und umfangreicher Erfahrung.

Wenn Sie noch nicht mit Intune vertraut sind und sich nicht sicher sind, wo Sie beginnen sollten, helfen Ihnen Sicherheitsgrundwerte, schnell ein sicheres Profil zu erstellen und bereitzustellen. Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Intune zu Verwaltungszwecken mit Sicherheitsgrundwerten viel einfacher, da sie in Intune integriert sind und moderne Verwaltungsfunktionen enthalten.

Weitere Informationen finden Sie [unter Windows Sicherheitsgrundwerte](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) und verwaltung [mobiler Geräte](https://docs.microsoft.com/windows/client-management/mdm/).

