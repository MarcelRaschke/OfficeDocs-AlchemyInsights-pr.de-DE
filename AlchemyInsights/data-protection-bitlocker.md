---
title: DataProtection – Bitlocker
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.custom:
- "9000220"
- "1802"
ms.openlocfilehash: 514f94a96fc2207db0ada5408d6d382671951bb1
ms.sourcegitcommit: c4e8c29a94f840816a023131ea7b4a2bf876c305
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/29/2022
ms.locfileid: "66435640"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlocker-Verschlüsselung mit Intune

Intune Endpoint Protection-Richtlinie kann verwendet werden, um Bitlocker-Verschlüsselungseinstellungen für Windows-Geräte zu konfigurieren. Weitere Informationen finden Sie [unter Windows 10 (und höher) Einstellungen zum Schutz von Geräten mit Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Zusätzlich zur Endpoint Protection-Richtlinie gibt es auch einen Verschlüsselungsbericht, der eine detailliertere Ansicht des Verschlüsselungsstatus für Geräte bietet. Auf diesen Bericht kann über das MEM-Portal unter **"Geräte > Überwachen**" zugegriffen werden, und dann unter **"Konfiguration** " wählen Sie " [Verschlüsselungsbericht](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)" aus.

Wenn Sie feststellen, dass Bitlocker nicht wie erwartet aktiviert werden kann oder sich das zum Aktivieren von Bitlocker verwendete Profil in einem Fehlerzustand befindet, lesen Sie den Verschlüsselungsbericht, um besser zu verstehen, warum das Verhalten auftritt.

Ausführliche Informationen zum Interpretieren des Berichts, einschließlich der verschiedenen Verschlüsselungsstatuswerte, finden Sie unter ["Geräteverschlüsselung mit Intune überwachen](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)".

Sie sollten beachten, dass viele neuere Geräte, auf denen Windows 10 ausgeführt werden, die automatische Bitlocker-Verschlüsselung unterstützen, die ohne anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung der Richtlinie auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Informationen finden Sie in den folgenden häufig gestellten Fragen(FAQ).

Informationen zur Problembehandlung bei Bitlocker-Problemen finden Sie [unter Problembehandlung für BitLocker-Richtlinien in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Häufig gestellte Fragen**

F: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?<br>
Antwort: Die Einstellungen in Intune Endpoint Protection-Richtlinie werden mithilfe des [Bitlocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) implementiert. Nicht alle Editionen oder Builds von Windows unterstützen den Bitlocker-CSP. <br><br>

F: Wie kann Bitlocker auf Geräten aktiviert werden, ohne dass eine Endbenutzerinteraktion erforderlich ist?<br>
Antwort: Solange die erforderlichen Voraussetzungen erfüllt sind, ist es möglich, Bitlocker "Silent Encryption" über Intune zu aktivieren. Details zu den Geräteanforderungen und Beispielrichtlinieneinstellungen zum Aktivieren der automatischen Verschlüsselung finden Sie im folgenden Dokument: [Automatisches Aktivieren der Bitlocker-Verschlüsselung](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist und die Standardeinstellungen des Betriebssystems für verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verwendet wird, löst das Anwenden einer Richtlinie mit anderen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen aus?<br>
A: Nein. Um die neuen Verschlüsselungseinstellungen anzuwenden, muss das Laufwerk zuerst entschlüsselt werden.<br><br>
**Hinweis:** Bei Geräten, die bei Autopilot registriert werden, wird die automatische Verschlüsselung, die während der Windows-Willkommensseite auftreten würde, erst ausgelöst, wenn Intune Richtlinie ausgewertet wird, wodurch die richtlinienbasierten Einstellungen anstelle der Betriebssystemstandards verwendet werden können.
 
F: Wenn ein Gerät aufgrund der Anwendung Intune Richtlinie verschlüsselt wird, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?<br>
A: Das Entfernen der verschlüsselungsbezogenen Richtlinie führt NICHT zur Entschlüsselung der konfigurierten Laufwerke.
 
F: Warum zeigt Intune Compliancerichtlinie an, dass auf meinem Gerät Bitlocker nicht aktiviert ist, obwohl dies der Grund ist?<br>
A: Die Einstellung "Bitlocker aktiviert" in der Intune Compliancerichtlinie verwendet den Windows Device Health Attestation (DHA)-Client. Dieser Client misst nur den Gerätestatus zum Startzeitpunkt. Wenn also ein Gerät seit Abschluss der Bitlocker-Verschlüsselung nicht neu gestartet wurde, meldet der DHA-Clientdienst Bitlocker nicht als aktiv.
 
 