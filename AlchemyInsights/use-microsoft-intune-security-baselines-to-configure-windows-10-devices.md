---
title: Verwenden der Microsoft Intune-Sicherheitsgrundsätze zum Konfigurieren von Windows 10-Geräten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: a82031e025d0bad6d364e438277709d16838e30f
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62740804"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Verwenden der Microsoft Intune-Sicherheitsgrundsätze zum Konfigurieren von Windows 10-Geräten

Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten. Sicherheitsgrundsätze sind vorkonfigurierte Gruppen von Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den relevanten Sicherheitsteams empfohlen werden. Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.

Wenn Sie Sicherheitsgrundsätze für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die unter Windows 10 oder höheren Versionen ausgeführt werden. Die Microsoft MDM-Sicherheitsgrundsätze (Verwaltung mobiler Geräte) zum Beispiel (1) aktiviert automatisch BitLocker für Wechsellaufwerke, (2) fordert das Kennwort zum Entsperren eines Geräts an und (3) deaktiviert die Basisauthentifizierung. Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, können Sie die Grundsätze anpassen, um die gewünschten Einstellungen anzuwenden.

Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren. Im Folgenden sind einige Vorteile dieser Funktionalität aufgeführt:
- Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen. Da Microsoft Intune mit dem Windows-Sicherheitsteam zusammenarbeitet, das die Grundsätze für Gruppenrichtlinien erstellt, basieren diese Empfehlungen auf soliden Richtlinien und umfangreichen Erfahrungen.
- Wenn Sie neu bei Microsoft Intune sind und nicht wissen, wo Sie anfangen sollen, helfen Ihnen die Sicherheitsgrundsätze dabei, schnell ein sicheres Profil zu erstellen und bereitzustellen.
- Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Microsoft Intune für Verwaltungszwecke mit Sicherheitsgrundsätzen viel einfacher, da diese Sicherheitsgrundsätze in Microsoft Intune integriert sind und modernste Funktionen für die Verwaltung enthalten.

Weitere Informationen finden Sie unter [Windows-Sicherheitsgrundsätze](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) und [Verwaltung mobiler Geräte (MDM)](https://docs.microsoft.com/windows/client-management/mdm/).