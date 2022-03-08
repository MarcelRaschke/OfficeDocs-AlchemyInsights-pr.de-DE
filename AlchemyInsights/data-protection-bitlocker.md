---
title: DataProtection – Bitlocker
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
ms.localizationpriority: medium
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b5ca78821068bbf85f1e1749ee6ce935ff58dfc
ms.sourcegitcommit: d11262728f0617a843a0117cb5172aa322022b27
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2022
ms.locfileid: "63185936"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der Bitlocker-Verschlüsselung mit Intune

Intune Endpoint Protection-Richtlinie kann verwendet werden, um BitLocker-Verschlüsselungseinstellungen für Windows-Geräte zu konfigurieren. Weitere Informationen finden Sie unter [Windows 10 -Einstellungen (und höher), um Geräte mit Intune zu schützen](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Zusätzlich zur Endpunktschutzrichtlinie gibt es auch einen Verschlüsselungsbericht, der eine detailliertere Ansicht des Verschlüsselungsstatus für Geräte bereitstellt. Auf diesen Bericht kann über das MEM-Portal unter **"Geräte > Monitor**" zugegriffen werden, und dann unter **"Konfiguration** wählen [Verschlüsselungsbericht" aus](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Wenn Sie feststellen, dass Bitlocker nicht wie erwartet aktiviert werden kann oder dass sich das Profil, das zum Aktivieren von BitLocker verwendet wird, in einem Fehlerzustand befindet, lesen Sie den Verschlüsselungsbericht, um ein besseres Verständnis des Verhaltens zu erhalten.

Ausführliche Informationen zur Interpretation des Berichts einschließlich der verschiedenen Verschlüsselungsstatuswerte finden Sie unter [Überwachen der Geräteverschlüsselung mit Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Beachten Sie, dass viele neuere Geräte unter Windows 10 die automatische Bitlocker-Verschlüsselung unterstützen, die ohne die Anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht standardmäßige Einstellungen konfiguriert sind. Weitere Informationen finden Sie in den folgenden häufig gestellten Fragen.

Informationen zur Problembehandlung von BitLocker-Problemen finden Sie unter [Problembehandlung für BitLocker-Richtlinien in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Häufig gestellte Fragen**

F: Welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpoint Protection-Richtlinie?<br>
A: Die Einstellungen in der Intune Endpoint Protection-Richtlinie werden mithilfe des [Bitlocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) implementiert. Nicht alle Editionen oder Builds von Windows unterstützen den Bitlocker-CSP. <br><br>

F: Wie kann BitLocker auf Geräten ohne Endbenutzerinteraktion aktiviert werden?<br>
Antwort: Solange die erforderlichen Voraussetzungen erfüllt sind, ist es möglich, bitlocker "Automatische Verschlüsselung" über Intune zu aktivieren. Details zu den Geräteanforderungen und Beispielrichtlinieneinstellungen zum Aktivieren der automatischen Verschlüsselung finden Sie im folgenden Dokument: [Automatisches Aktivieren der Bitlocker-Verschlüsselung](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

F: Wenn ein Gerät bereits mit Bitlocker verschlüsselt ist, indem die Standardeinstellungen des Betriebssystems für verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verwendet werden, löst das Anwenden einer Richtlinie mit anderen Einstellungen automatisch die erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen aus?<br>
A: Nein. Um die neuen Verschlüsselungseinstellungen anzuwenden, muss das Laufwerk zuerst entschlüsselt werden.<br><br>
**Hinweis:** Bei Geräten, die bei Autopilot registriert sind, wird die automatische Verschlüsselung, die während der Windows-Willkommensseite auftreten würde, erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, sodass die richtlinienbasierten Einstellungen anstelle der Standardeinstellungen des Betriebssystems verwendet werden können.
 
F: Wenn ein Gerät aufgrund der Anwendung der Intune-Richtlinie verschlüsselt ist, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?<br>
A: Das Entfernen verschlüsselungsbezogener Richtlinien führt NICHT zur Entschlüsselung der konfigurierten Laufwerke.
 
F: Warum zeigt die Intune-Compliancerichtlinie, dass bitlocker auf meinem Gerät nicht aktiviert ist, obwohl dies der Typ ist?<br>
A: Die Einstellung "Bitlocker aktiviert" in der Intune-Compliancerichtlinie verwendet den Windows Device Health Attestation (DHA)-Client. Dieser Client misst nur den Gerätestatus beim Start. Wenn ein Gerät also seit Abschluss der Bitlocker-Verschlüsselung nicht neu gestartet wurde, meldet der DHA-Clientdienst Bitlocker nicht als aktiv.
 
 