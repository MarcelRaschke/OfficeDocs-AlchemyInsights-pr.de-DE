---
title: Begriffe, die in SharePoint Online-Ausdrucks-Store fehlen
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
ms.openlocfilehash: 6e34b70a424ea6f435af24672ea276757a930b37
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63189680"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlocker-Verschlüsselung mit Intune

Intune Endpoint Protection-Richtlinie kann verwendet werden, um Boitlocker-Verschlüsselungseinstellungen für Windows Geräte zu konfigurieren, wie unter : Windows10 -Einstellungen (und höher) zum Schützen von Geräten mit Intune

Beachten Sie, dass viele neuere Geräte, auf denen Windows 10 ausgeführt werden, die automatische BitLocker-Verschlüsselung unterstützen, die ohne die Anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Informationen finden Sie in den häufig gestellten Fragen.


Häufig gestellte Fragen: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?
A: Die Einstellungen in Intune Endpoint Protection-Richtlinie werden mithilfe des Bitlocker-CSP implementiert.  Nicht alle Editionen oder Builds von Windows unterstützen den Bitlocker-CSP. Zu diesem Zeitpunkt Windows Editionen: Enterprise; Education, Mobile, Mobile Enterprise und Professional (ab Build 1809) werden unterstützt.




F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist, indem die Standardeinstellungen des Betriebssystems für die Verschlüsselungsmethode verwendet werden und die Verschlüsselungsstärke (XTS-AES-128) eine Richtlinie mit anderen Einstellungen anwendet, wird automatisch die erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?

A: Nein. Um die neuen Verschlüsselungseinstellungen anzuwenden, muss das Laufwerk zuerst entschlüsselt werden.

Hinweis Für Geräte, die bei Autopilot registriert sind, wird die automatische Verschlüsselung, die während der Windows-Willkommensseite auftreten würde, erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, sodass die richtlinienbasierten Einstellungen anstelle der Standardeinstellungen des Betriebssystems verwendet werden können.




F Wenn ein Gerät aufgrund der Anwendung der Intune-Richtlinie verschlüsselt ist, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?

A: Das Entfernen der verschlüsselungsbezogenen Richtlinie führt NICHT zur Entschlüsselung der Laufwerke, die konfiguriert wurden.




F: Warum zeigt die Intune-Compliancerichtlinie an, dass auf meinem Gerät "Bitlocker aktiviert" nicht aktiviert ist, aber es ist?

Antwort: Die Einstellung "BitLocker aktiviert" in der Intune-Compliancerichtlinie verwendet den Windows Client für den Integritätsnachweis (Device Health Attestation, DHA). Dieser Client misst nur den Gerätestatus beim Start. Wenn ein Gerät also nicht neu gestartet wurde, seit die BitLocker-Verschlüsselung abgeschlossen wurde, meldet der DHA-Clientdienst bitlocker nicht als aktiv.