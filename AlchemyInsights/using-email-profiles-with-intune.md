---
title: Verwenden von E-Mail-Profilen mit Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 6ce0d622c6e8db2ed0100593559bc0fff2ba9e1c
ms.sourcegitcommit: c26373c21c837937b41026f56fedfc51b7b80ea7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2022
ms.locfileid: "61970203"
---
# <a name="using-email-profiles-with-intune"></a>Verwenden von E-Mail-Profilen mit Intune

Intune kann verwendet werden, um E-Mail-Profile für den nativen (integrierten) E-Mail-Client auf mehreren Geräteplattformen zu erstellen und bereitzustellen.

Informationen über einige der Einschränkungen, die mit E-Mail-Profilen verbunden sind, einschließlich der Verarbeitung vorhandener Profile und der Entfernung von E-Mail-Profilen, finden Sie unter [Hinzufügen von E-Mail-Einstellungen für Geräte mit Intune](https://docs.microsoft.com/intune/email-settings-configure).

Weitere Informationen zum Erstellen von E-Mail-Profilen für jede Geräteplattform finden Sie unter:

[Android-Geräteeinstellungen zum Konfigurieren von E-Mail, Authentifizierung und Synchronisierung in Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Hinzufügen von E-Mail-Einstellungen für iOS- und iPadOS-Geräte in Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[E-Mail-Profileinstellungen in Microsoft Intune für Windows Phone 8.1-Geräte](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[E-Mail-Profileinstellungen für Geräte in Microsoft Intune, die unter Windows 10 ausgeführt werden](https://docs.microsoft.com/intune/email-settings-windows-10)

**Häufig auftretendes Synchronisierungsproblem**

**Ein KNOX unter Android-E-Mail-Profil verhindert, dass die Kontakte, Kalender und Aufgaben des Benutzers mit den Geräten des Benutzers synchronisiert werden.**

Das KNOX unter Android KNOX-E-Mail-Profil bietet dem Administrator die Möglichkeit zu entscheiden, welche Inhaltstypen mit dem Gerät synchronisiert werden, indem die gewünschten Inhaltstypen auf "Aktiviert" festgelegt werden.

Wenn die Einstellung für einen der Inhaltstypen auf **Nicht konfiguriert** (Standardeinstellung) festgelegt ist, wird dieser Inhaltstyp nicht automatisch synchronisiert. Ein Benutzer könnte den gewünschten Inhaltstyp direkt auf dem Gerät manuell aktivieren, aber diese Konfiguration wird durch die Intune-Richtlinieneinstellung außer Kraft gesetzt, und die Synchronisierung wird für diesen Inhaltstyp beendet.

