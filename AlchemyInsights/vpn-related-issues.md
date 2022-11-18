---
title: Probleme mit dem VPN
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
- "1545"
ms.date: 07/28/2020
ms.openlocfilehash: 942b8b7830f9d5122ffbb424a8b9633e81c61f11
ms.sourcegitcommit: 5fb344efe019d0f7e641a59b2bd0535e6cbafb72
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66527844"
---
# <a name="vpn-related-issues"></a>Probleme mit dem VPN

Die erfolgreiche Implementierung von VPN-Konnektivität für MDM-Clients hängt von einem bereitgestellten Profil ab, das die Anforderungen der VPN-Infrastruktur korrekt widerspiegelt. Die entsprechenden Einstellungen für die von Ihnen untersuchten Clientplattformen finden Sie unter: 

[Geräteeinstellungen für Windows 10 und Windows Holographic zum Hinzuzufügen von VPN-Verbindungen mithilfe von Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Hinzufügen von VPN-Einstellungen auf iOS- und iPadOS-Geräten in Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Android-Geräteeinstellungen zur VPN-Konfiguration in Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Hinzufügen von VPN-Einstellungen auf macOS-Geräten in Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)
[Verwenden einer VPN- und app-basierten VPN-Richtlinie auf Android-Enterprise-Geräten in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/app-configuration-vpn-ae)

Wenn Ihr VPN-Profil zertifikatsbasierte Authentifizierung verwendet, stellen Sie sicher, dass die mit dem VPN-Profil verknüpften Stammzertifikat- und Clientauthentifizierungszertifikat-Profile erfolgreich bereitgestellt werden.

**Häufig auftretende Probleme**

**Ich habe ein VPN-Profil auf einem Gerät bereitgestellt. Intune zeigt an, dass dies erfolgreich war, aber das Gerät verbindet sich nicht mit dem VPN.**

Der Status "Erfolgreich" bedeutet, dass Intune das Profil wie konfiguriert erfolgreich bereitgestellt hat. Diese Konfigurationen entsprechen aber möglicherweise nicht Ihren Netzwerk- und/oder Authentifizierungsanforderungen. Überprüfen Sie die Protokolle in der Infrastruktur und im Authentifizierungsdienst (auf dem VPN-Server und dem NPS/Radius-Server), um weitere Einzelheiten über die versuchte Verbindung zu erfahren. Möglicherweise müssen Sie mit Ihrem Netzwerkinfrastruktur-Team oder dem VPN-Drittanbietern zusammenarbeiten, um Protokolle zu erfassen und zu überprüfen.

**Wenn ich ein benutzerdefiniertes VPN für iOS konfiguriere, wird das Feature "Pro-App-VPN" nicht zur Verfügung gestellt.**

Pro-App-VPN für iOS-Geräte in Intune steht derzeit für eine bestimmte Liste von Anbietern und Partnern zur Verfügung, die vor der Konfiguration eines Pro-App-VPNs auch die Zertifikatvoraussetzungen erfüllen müssen. Weitere Informationen finden Sie unter [Einrichten eines Pro-App-VPN für iOS/iPadOS-Geräte in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) einrichten.

Weitere Informationen zu allen VPN-Verbindungstypen in Intune finden Sie unter [Erstellen von VPN-Profilen zum Herstellen einer Verbindung mit VPN-Servern in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand-VPN wird nicht ausgelöst, wenn auf eine konfigurierte Domäne zugegriffen wird**

Um die automatischen VPN-Einstellungen zu testen, legen Sie die folgenden Werte fest:

Ich möchte Folgendes tun: **Jeden Verbindungsversuch auswerten**

Auswählen, ob eine Verbindung hergestellt werden soll: **Verbinden, falls erforderlich**

Wenn Benutzer auf diese Domänen zugreifen: **Ziel** *Domänenname*

Wenn die vorstehende Konfiguration nicht erfolgreich ist, fügen Sie das folgende Element hinzu:

Wenn diese URL nicht erreichbar ist, VPN-Verbindung erzwingen: **BADURL**
