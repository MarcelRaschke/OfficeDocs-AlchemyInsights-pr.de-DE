---
title: Ausdrücke, die im SharePoint Online-Terminologiespeicher fehlen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "5200021"
- "1243"
ms.date: 04/21/2020
ms.openlocfilehash: 9678e4dad626f5624bd9d14a72f8e81c17c337f1
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66255394"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlocker-Verschlüsselung mit Intune

Intune Endpoint Protection-Richtlinie kann verwendet werden, um Boitlocker-Verschlüsselungseinstellungen für Windows-Geräte zu konfigurieren, wie unter : Windows10 -Einstellungen (und höher) beschrieben, um Geräte mit Intune

Sie sollten sich bewusst sein, dass viele neuere Geräte, auf denen Windows 10, die automatische Bitlocker-Verschlüsselung unterstützen, die ohne anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung der Richtlinie auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Details finden Sie in den häufig gestellten Fragen.


Häufig gestellte Fragen F: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?
A: Die Einstellungen in Intune Endpoint Protection-Richtlinie werden mithilfe des Bitlocker-CSP implementiert.  Nicht alle Editionen oder Builds von Windows unterstützen den Bitlocker-CSP. Zu diesem Zeitpunkt Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise und Professional (ab Build 1809) werden unterstützt.




F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist und die Standardeinstellungen des Betriebssystems für verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verwendet wird, wird durch anwenden einer Richtlinie mit unterschiedlichen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?

A: Nein. Um die neuen Verschlüsselungseinstellungen anwenden zu können, muss das Laufwerk zuerst entschlüsselt werden.

Hinweis Für Geräte, die bei Autopilot registriert werden, wird die automatische Verschlüsselung, die während der Windows-Willkommensseite auftreten würde, erst ausgelöst, wenn Intune Richtlinie ausgewertet wird, wodurch die richtlinienbasierten Einstellungen anstelle der Betriebssystemstandards verwendet werden können.




F Wenn ein Gerät aufgrund der Anwendung Intune Richtlinie verschlüsselt wird, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?

A: Das Entfernen der verschlüsselungsbezogenen Richtlinie führt NICHT zur Entschlüsselung der konfigurierten Laufwerke.




F: Warum zeigt die Intune-Compliancerichtlinie an, dass mein Gerät nicht über "Bitlocker Enabled" verfügt, aber es ist?

A: Die Einstellung "Bitlocker aktiviert" in der Intune-Compliancerichtlinie verwendet den Windows Device Health Attestation (DHA)-Client. Dieser Client misst nur den Gerätestatus zum Startzeitpunkt. Wenn also ein Gerät seit Abschluss der Bitlocker-Verschlüsselung nicht neu gestartet wurde, meldet der DHA-Clientdienst BitLocker nicht als aktiv.