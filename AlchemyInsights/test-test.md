---
title: Begriffe, die in SharePoint Onlineausdrucks-Store fehlen
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 164993b782546526cc591d661835ff0a88fe3304
ms.sourcegitcommit: de17cf643683f8406831eecaf6299ace609f5599
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2022
ms.locfileid: "65721041"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlocker-Verschlüsselung mit Intune

Intune Endpoint Protection-Richtlinie kann verwendet werden, um Boitlocker-Verschlüsselungseinstellungen für Windows Geräte zu konfigurieren, wie unter : Windows10 -Einstellungen (und höher) beschrieben, um Geräte mithilfe von Intune

Sie sollten sich bewusst sein, dass viele neuere Geräte, auf denen Windows 10, die automatische Bitlocker-Verschlüsselung unterstützen, die ohne anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung der Richtlinie auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Details finden Sie in den häufig gestellten Fragen.


Faq F: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?
A: Die Einstellungen in Intune Endpoint Protection-Richtlinie werden mithilfe des Bitlocker-CSP implementiert.  Weder alle Editionen noch Builds von Windows unterstützen den Bitlocker-CSP. Zu diesem Zeitpunkt Windows Editionen: Enterprise; Education, Mobile, Mobile Enterprise und Professional (ab Build 1809) werden unterstützt.




F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist und die Standardeinstellungen des Betriebssystems für verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verwendet wird, wird durch anwenden einer Richtlinie mit unterschiedlichen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?

A: Nein. Um die neuen Verschlüsselungseinstellungen anwenden zu können, muss das Laufwerk zuerst entschlüsselt werden.

Hinweis Für Geräte, die bei Autopilot registriert werden, wird die automatische Verschlüsselung, die während der Windows-Willkommensseite auftreten würde, erst ausgelöst, wenn Intune Richtlinie ausgewertet wird, wodurch die richtlinienbasierten Einstellungen anstelle der Betriebssystemstandards verwendet werden können.




F Wenn ein Gerät aufgrund der Anwendung Intune Richtlinie verschlüsselt wird, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?

A: Das Entfernen der verschlüsselungsbezogenen Richtlinie führt NICHT zur Entschlüsselung der konfigurierten Laufwerke.




F: Warum zeigt die Intune-Compliancerichtlinie an, dass mein Gerät nicht über "Bitlocker Enabled" verfügt, aber es ist?

Antwort: Die Einstellung "Bitlocker aktiviert" in der Intune-Compliancerichtlinie verwendet den Windows DHA-Client (Device Health Attestation). Dieser Client misst nur den Gerätestatus zum Startzeitpunkt. Wenn also ein Gerät seit Abschluss der Bitlocker-Verschlüsselung nicht neu gestartet wurde, meldet der DHA-Clientdienst BitLocker nicht als aktiv.