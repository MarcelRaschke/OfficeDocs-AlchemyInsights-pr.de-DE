---
title: Intune Win32 App-Bereitstellung
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 104f135cd981f1ba05b038475ced9b09501f122b
ms.sourcegitcommit: 49eaa1417714617d768df85fd79b65e35b6e5c83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/11/2022
ms.locfileid: "62604191"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 App-Bereitstellung

Mit Microsoft Intune können Win32-Anwendungen, einschließlich aber nicht beschränkt auf MSI und .EXE, auf Windows 10-Geräten bereitgestellt werden. Für den verwendeten Bereitstellungsmechanismus muss die Intune-Verwaltungserweiterung (IME) auf dem Zielgerät installiert sein. Die IME wird automatisch installiert, wenn ein PowerShell-Skript ausgeführt wird, oder eine Win32-Anwendung für einen Benutzer/auf ein Benutzergerät bereitgestellt wird.

Es gibt außerdem eine Reihe an Voraussetzungen, die für die Bereitstellung von Win32-Apps erfüllt werden müssen. Dazu gehören:

- Unterstützte Plattformen: Windows 10 Version 1607 oder später (Enterprise, Pro, und Education-Versionen).
- Unterstützte Architektur: x86 und x64.
- Geräteverwaltung: ADD eingebunden und automatisch registriert (darunter Hybriddomäne eingebunden und Gruppenrichtlinie automatisch registriert).
- Format des Anwendungspakets: Die .**intunewin** -Datei wird von dem [Tool zur Vorbereitung von Microsoft Win32-Inhalten](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare) vorbereitet.
- Einschränkungen:
    - Maximale Größe: 8 GB.
    - Nicht unterstützte Architektur: ARMs.

Lesen Sie das Dokument „[Eine Win32-App in Microsoft Intune hinzufügen, zuweisen und überwachen](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)“, um weitere Informationen zu diesen Schritten zu erhalten.

Genauere Informationen zur Problembehandlung der Anwendungsbereitstellung auf Windows, einschließlich der Bereitstellung von Win32-Apps, erhalten Sie in den folgenden Dokumenten

- [Behandeln von Problemen bei der App-Installation](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Problembehandlung bei Win32-Apps](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)