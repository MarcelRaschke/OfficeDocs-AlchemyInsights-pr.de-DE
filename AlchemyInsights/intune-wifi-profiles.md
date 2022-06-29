---
title: Intune-WLAN-Profile
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: high
ms.custom:
- "9000076"
- "1548"
ms.date: 07/28/2020
ms.openlocfilehash: f3ebea1ad277a182181ef0d9fe26bfef95928de2
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66321159"
---
# <a name="intune-wi-fi-profiles"></a>Intune-WLAN-Profile

Die erfolgreiche Implementierung von WLAN-Konnektivität für MDM-Clients hängt von einem korrekt bereitgestellten Profil ab, das die Anforderungen der WLAN-Infrastruktur des Unternehmens widerspiegelt. Informationen zum Überprüfen der entsprechenden Einstellungen für die Clientplattformen, die Sie untersuchen, finden Sie unter: 

[Hinzufügen von WLAN-Einstellungen für Geräte, die Android in Microsoft Intune ausführen](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Hinzufügen von WLAN-Einstellungen für Android Enterprise-dedizierte und vollständig verwaltete Geräte in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Hinzufügen von WLAN-Einstellungen für iOS- und iPadOS-Geräte in Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Hinzufügen von WLAN-Einstellungen für Windows 10-Geräte und Geräte mit einer höheren Windows-Version in Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importieren von WLAN-Einstellungen für Windows-Geräte in Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Häufig auftretende Probleme**

**Ich stellen ein WLAN-Profil bereit, das von einem bereitgestellten Zertifikat abhängig ist, das im WLAN-Profil angegeben ist. Die Konfigurationsprofile weisen jedoch einen Fehlerstatus auf.**

Überprüfen Sie, ob Ihr Gerät das Zertifikat erhalten hat.

1. Wechseln Sie in Intune zu **Alle Geräte**, und wählen Sie das Gerät > **Gerätekonfiguration** aus.

2. Überprüfen Sie, ob alle erwarteten Profile aufgeführt sind und einen erfolgreichen Zustand aufweisen.

3. Wenn Sie bei einem Android-Profil Zwischenzertifikate in Ihrer Zertifikatkette besitzen, müssen Sie sicherstellen, dass diese auf Android-Geräten bereitgestellt sind.

    Um den Zertifikatstatus zu überprüfen, wechseln Sie zu **Gerätekonfiguration** > **Profile** > **Android-Zwischenzertifizierungsstelle** > **Eigenschaften** > **vertrauenswürdiges Zertifikat**.

Wenn weiterhin Fehler angezeigt werden, lesen Sie die Abschnitte zur Verfahren und zur Problembehandlung. Weitere Informationen finden Sie unter [Übersicht für die Problembehandlung von SCEP-Zertifikatprofilen mit Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Ich habe ein WLAN-Profil auf einem Gerät bereitgestellt. Intune zeigt an, dass dies erfolgreich war, aber das Gerät verbindet sich nicht mit dem WLAN.**

Der Status "Erfolgreich" bedeutet, dass Intune das Profil wie konfiguriert erfolgreich bereitgestellt hat. Diese Konfigurationen entsprechen aber möglicherweise nicht Ihren Netzwerk- und/oder Authentifizierungsanforderungen. Weitere Einzelheiten zu der versuchten Verbindung finden Sie in den Protokollen in der Infrastruktur und im Authentifizierungsdienst (auf dem WLAN-Zugriffspunktcontroller und dem NPS/Radius-Server). Möglicherweise müssen Sie mit Ihrem Netzwerkinfrastrukturteam oder dem WLAN-Drittanbieterhersteller zusammenarbeiten, um Protokolle zu sammeln und zu überprüfen.