---
title: Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9006500"
- "11142"
ms.date: 06/04/2021
ms.openlocfilehash: 58ffb3c97cec25f3c3318c33b36aad4696d0af0f
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66308880"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten

Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten. Sicherheitsbaselines sind vorkonfigurierte Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den relevanten Sicherheitsteams empfohlen werden. Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.

Wenn Sie Sicherheitsbaselines für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die auf Windows 10 oder höher ausgeführt werden. Beispielsweise aktiviert die Sicherheitsbaseline für die Verwaltung mobiler Geräte (MDM) von Microsoft BitLocker automatisch für Wechseldatenträger, erfordert das Kennwort zum Entsperren eines Geräts und deaktiviert die Standardauthentifizierung. Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, können Sie die Grundsätze anpassen, um die gewünschten Einstellungen anzuwenden.

Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren. Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen. Intune arbeitet mit dem Windows-Sicherheitsteam zusammen, das Basispläne für Gruppenrichtlinien erstellt, sodass diese Empfehlungen auf solider Anleitung und umfangreicher Erfahrung basieren.

Wenn Sie noch nicht mit Intune und unsicher sind, wo Sie beginnen sollen, helfen Ihnen Sicherheitsgrundwerte dabei, schnell ein sicheres Profil zu erstellen und bereitzustellen. Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Intune zu Verwaltungszwecken mit Sicherheitsbaselines viel einfacher, da sie in Intune integriert sind und moderne Verwaltungsfunktionen enthalten.

Weitere Informationen finden Sie unter [Windows-Sicherheitsgrundwerte](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) und [Mobile Geräteverwaltung](https://docs.microsoft.com/windows/client-management/mdm/).
