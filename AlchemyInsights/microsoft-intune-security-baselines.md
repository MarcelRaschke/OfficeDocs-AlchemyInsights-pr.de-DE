---
title: Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 7672028fd9fd0d96ac64bd0c474cfed127ef9669
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63264581"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten

Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten. Sicherheitsgrundwerte sind Windows vorkonfigurierte Gruppen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den entsprechenden Sicherheitsteams empfohlen werden. Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.

Wenn Sie Sicherheitsgrundwerte für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die auf Windows 10 oder höher ausgeführt werden. Beispielsweise aktiviert die Microsoft Mobile Device Management (MDM)-Sicherheitsbaseline BitLocker automatisch für Wechseldatenträger, erfordert das Kennwort zum Entsperren eines Geräts und deaktiviert die Standardauthentifizierung. Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, können Sie die Grundsätze anpassen, um die gewünschten Einstellungen anzuwenden.

Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren. Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen. Intune arbeitet mit dem Windows Sicherheitsteam zusammen, das Basispläne für Gruppenrichtlinien erstellt, sodass diese Empfehlungen auf soliden Anleitungen und umfangreicher Erfahrung basieren.

Wenn Sie noch nicht mit Intune vertraut sind und sich nicht sicher sind, wo Sie beginnen sollten, helfen Ihnen Sicherheitsgrundwerte, schnell ein sicheres Profil zu erstellen und bereitzustellen. Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Intune zu Verwaltungszwecken mit Sicherheitsgrundwerten viel einfacher, da sie in Intune integriert sind und moderne Verwaltungsfunktionen enthalten.

Weitere Informationen finden Sie [unter Windows Sicherheitsgrundwerte](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) und verwaltung [mobiler Geräte](https://docs.microsoft.com/windows/client-management/mdm/).

